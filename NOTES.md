# System context — kernel and userspace
                ┌────────────────────────────┐
                │        Linux Kernel        │
                │         (2003 era)         │
                └───────────┬────────────────┘
                            │
                            │  sends environment to /sbin/hotplug
                            │  (before netlink uevents existed)
                            │
                            ▼
                   /sbin/hotplug  → invokes  →  /sbin/udev
                         (kernel passes env vars)

Environment variables from kernel:
ACTION=add
DEVPATH=/class/block/sda
SUBSYSTEM=block
SEQNUM=123


# Entry point: main() (in udev.c)
┌────────────────────────────────────────────────────────┐
│ int main(int argc, char **argv, char **envp)           │
├────────────────────────────────────────────────────────┤
│ argv[1] = subsystem ("block", "class", "net", ...)     │
│                                                        │
│ main_envp → saved globally                             │
│                                                        │
│ get_action()  → getenv("ACTION")                       │
│ get_devpath() → getenv("DEVPATH")                      │
│ get_seqnum()  → getenv("SEQNUM")                       │
│                                                        │
│ get_dirs() → determine:                                │
│   • sysfs mount path (/sys)                            │
│   • udev_root (/dev)                                   │
│   • udev_db_filename (/etc/udev/udev.tdb)              │
│   • udev_config_filename (/etc/udev/udev.config)       │
│   • udev_config_permission_filename                    │
│                                                        │
│ udevdb_init(UDEVDB_DEFAULT) → open TDB file            │
│ namedev_init() → load udev.config rules                │
│                                                        │
│ if ACTION=="add"    → udev_add_device()                │
│ if ACTION=="remove" → udev_remove_device()             │
│                                                        │
│ udevdb_exit() → close db                               │
└────────────────────────────────────────────────────────┘


# Add-device path (udev_add_device())
                   +----------------------------------+
                   | int udev_add_device(path, subsys)|
                   +----------------------------------+
                                     │
                                     ▼
          ┌──────────────────────────────────────────┐
          │ sleep_for_dev(path)                      │
          │ └─ wait up to 10s for /sys/<path>/dev    │
          │    (the kernel writes "major:minor" there)│
          └──────────────────────────────────────────┘
                                     │
                                     ▼
          ┌──────────────────────────────────────────┐
          │ get_class_dev(path)                      │
          │ └─ build full sysfs path = /sys + DEVPATH │
          │ └─ sysfs_open_class_device()              │
          │      → returns struct sysfs_class_device* │
          └──────────────────────────────────────────┘
                                     │
                                     ▼
          ┌──────────────────────────────────────────┐
          │ namedev_name_device(class_dev, &dev)     │
          │ └─ parses udev.config                    │
          │    - matches BUS/vendor/serial/rules     │
          │    - fills dev.name = "camera", etc.     │
          └──────────────────────────────────────────┘
                                     │
                                     ▼
          ┌──────────────────────────────────────────┐
          │ get_major_minor(class_dev, &maj, &min)   │
          │ └─ read class_dev->"dev" attribute        │
          │ └─ sscanf("8:0", "%u:%u") → maj=8, min=0 │
          └──────────────────────────────────────────┘
                                     │
                                     ▼
          ┌──────────────────────────────────────────┐
          │ udevdb_add_dev(path, &dev)               │
          │ └─ store in TDB: key=DEVPATH, val=struct │
          │    so removal can later look it up       │
          └──────────────────────────────────────────┘
                                     │
                                     ▼
          ┌──────────────────────────────────────────┐
          │ create_node(&dev)                        │
          │ ├─ combine root + name → /dev/<dev.name> │
          │ ├─ determine node type:                  │
          │    'b' → S_IFBLK, 'c' → S_IFCHR, etc.    │
          │ ├─ res = makedev(major, minor)           │
          │ ├─ mknod("/dev/<name>", mode, res)       │
          │ └─ (TODO: chown/chmod)                   │
          └──────────────────────────────────────────┘
                                     │
                                     ▼
                            Device node created


# Remove-device path (udev_remove_device())
+-------------------------------------------------------+
| int udev_remove_device(char *device, char *subsystem) |
+-------------------------------------------------------+
                     │
                     ▼
       ┌──────────────────────────────────────────────┐
       │ get_name(device, major, minor)               │
       │ ├─ lookup DEVPATH in udev.tdb                │
       │ ├─ if not found, fallback to basename(path)  │
       │ └─ return "sda", "camera", etc.              │
       └──────────────────────────────────────────────┘
                     │
                     ▼
       ┌──────────────────────────────────────────────┐
       │ udevdb_delete_dev(device)                    │
       │ └─ delete key=DEVPATH from TDB               │
       └──────────────────────────────────────────────┘
                     │
                     ▼
       ┌──────────────────────────────────────────────┐
       │ delete_node(name)                            │
       │ └─ unlink("/dev/<name>")                     │
       └──────────────────────────────────────────────┘

# Configuration flow (udev.config + namedev.c)
/etc/udev/udev.config
 ├─ LABEL, BUS="usb", vendor="FUJIFILM", NAME="camera"
 ├─ NUMBER, BUS="pci", id="00:0b.0", NAME="dsp"
 ├─ TOPOLOGY, BUS="usb", place="1.3", NAME="mouse0"
 └─ REPLACE, KERNEL="ttyUSB1", NAME="visor"

When namedev_name_device() runs:
parse lines → match criteria with sysfs attributes:
   BUS        → "usb", "pci", etc.
   vendor/id  → read from /sys/.../vendor
   place/id   → read topology path
   kernel     → current device name
if rule matches → copy NAME="..." → dev.name

# Database layer (udevdb.c)
File: /etc/udev/udev.tdb (Trivial DB)
-------------------------------------
KEY   = DEVPATH (/class/block/sda)
VALUE = struct udevice {
           name="camera",
           major=8,
           minor=0,
           type='b'
        }
-------------------------------------
Used for:
  • remove lookups
  • re-creating devices after reboot

APIs:
udevdb_init(UDEVDB_DEFAULT)
udevdb_add_dev(path, &dev)
udevdb_get_dev(path)
udevdb_delete_dev(path)
udevdb_exit()

Internally uses:
TDB_DATA key, data;
tdb_store();
tdb_fetch();
tdb_delete();

# Filesystem and data flow (visual)
┌──────────┐
│ /sys     │
│ (sysfs)  │
│ ├─ /class/block/sda/dev   → "8:0"     ← kernel exports
│ ├─ /class/block/sda/vendor → "FUJIFILM"
│ └─ ...                                    ↑
└──────────┘                                │
      │                                     │
      ▼                                     │
┌──────────┐     read by libsysfs           │
│  udev    │────────────────────────────────┘
│  udev-add.c
│   → reads "dev" → major/minor
│   → applies udev.config rules
│   → creates /dev/<name>
│   → logs into udev.tdb
└──────────┘
      │
      ▼
┌──────────┐
│ /dev     │
│ ├─ camera (block 8:0)
│ ├─ dsp
│ ├─ lp_epson
│ └─ visor
└──────────┘




# Timing and interaction (whole picture)
        [Kernel adds USB camera]
                │
                ▼
        (1) /sbin/hotplug ACTION=add DEVPATH=/class/block/sda
                │
                ▼
        (2) udev.c
                │
                ▼
        (3) udev_add_device()
                │
                ├─ wait for /sys/.../dev
                ├─ open sysfs_class_device
                ├─ parse /etc/udev/udev.config
                ├─ assign name="camera"
                ├─ read "dev" → 8:0
                ├─ mknod("/dev/camera", S_IFBLK, makedev(8,0))
                └─ write {path→device} into udev.tdb
                │
                ▼
        (4) user sees /dev/camera

If later unplugged:
Kernel → ACTION=remove DEVPATH=/class/block/sda
  → udev_remove_device()
      → look up in DB
      → unlink("/dev/camera")
      → delete DB record


# Architectural summary
┌───────────────────────────────────────────────────────────┐
│                UDEV (v0.005, Oct 2003)                    │
│───────────────────────────────────────────────────────────│
│  • Stateless helper per hotplug event                     │
│  • Reads sysfs via libsysfs                                │
│  • Configurable naming via udev.config                    │
│  • Persists info in udev.tdb (Trivial DB)                 │
│  • Calls mknod() and unlink() directly                    │
│  • No daemons, no netlink, no parallel queue              │
│  • Replaces kernel devfs (deprecated)                     │
└───────────────────────────────────────────────────────────┘


# Summary of the early udev flow (compact view)
Kernel → /sbin/hotplug
      ENV: ACTION=add, DEVPATH=/class/block/sda
          │
          ▼
       udev.c
          │
          ├─ get_action(), get_devpath()
          ├─ get_dirs() → set paths
          ├─ udevdb_init()
          ├─ namedev_init() → load config
          │
          └─ udev_add_device()
                │
                ├─ wait for /sys/dev
                ├─ read major/minor
                ├─ apply naming rule
                ├─ mknod("/dev/name", mode, dev_t)
                ├─ add to udev.tdb
                └─ exit

# Evolution (for perspective)
| Generation  | Implementation               | Key Mechanism                     |
| ----------- | -----------------------------| --------------------------------- |
|     (2003)  | `udev` (this one)            | Hotplug env → one-shot program    |
|     (2005)  | `udevd` daemon               | Netlink uevents, async processing |
|     (2010)  | `udevd` + `udevadm`          | unified CLI, rule engine          |
|     (2011+) | inside systemd (`src/udev/`) | socket activation, Cgroups, etc.  |


