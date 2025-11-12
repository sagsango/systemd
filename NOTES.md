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


# Flowchart
                              +----------------------------+
                              |     Kernel (2.6)           |
                              |  sysfs + hotplug           |
                              +----------------------------+
                                        |
                                        | netlink/hotplug event
                                        | ACTION=add/remove
                                        | DEVPATH=/class/usb/host1
                                        | SUBSYSTEM=usb
                                        v
                   +-------------------------------------------+
                   | /etc/hotplug.d/default/udev.hotplug       |
                   | (symlink → /sbin/udev)                    |
                   +-------------------------------------------+
                                        |
                                        | execve("/sbin/udev", ["udev", "subsystem"], env)
                                        v
                   +-------------------------------------------+
                   |                /sbin/udev                 |
                   |             main() in udev.c              |
                   +-------------------------------------------+
                                        |
                                        | 1. Check argc == 2 → subsystem = argv[1]
                                        | 2. getenv("ACTION") → "add" or "remove"
                                        | 3. getenv("DEVPATH") → e.g. "/class/usb/host1"
                                        | 4. getenv("SEQNUM")
                                        |
                                        | Filter:
                                        |   • Must contain "class" or "block"
                                        |   • NOT subsystem "net"
                                        |
                                        v
                   +-------------------------------------------+
                   |             get_dirs()                    |
                   | • Detect sysfs mount (/proc/mounts)       |
                   | • Override via env:                       |
                   |     UDEV_SYSFS_PATH, UDEV_ROOT, etc.      |
                   | • Build paths:                            |
                   |     udev_root = "/dev" (default)          |
                   |     udev_db_filename = "/etc/udev/udev.tdb"|
                   +-------------------------------------------+
                                        |
                                        v
                   +-------------------------------------------+
                   |          udevdb_init(UDEVDB_DEFAULT)      |
                   |     → tdb_open("/etc/udev/udev.tdb")      |
                   |       (Trivial Database - persistent)     |
                   +-------------------------------------------+
                                        |
                 +-------------------------------+-----------------------+
                 |                               |                       |
                 v                               v                       v
        ACTION="add"                   ACTION="remove"           unknown → exit(-EINVAL)
                 |                               |
                 v                               v
        +----------------+             +-------------------------+
        | udev_add_device()            | udev_remove_device()    |
        | (udev-add.c)                 | (udev-remove.c)         |
        +----------------+             +-------------------------+
                 |                               |
                 | 1. sleep_for_dev()            | 1. get_name(path,0,0)
                 |    → wait up to 10s for       |    → lookup in TDB
                 |       /sys/.../dev file        |       if found → dev->name
                 |                               |       else → basename(DEVPATH)
                 | 2. get_class_dev()            |
                 |    → sysfs_open_class_device()|
                 |                               | 2. udevdb_delete_dev(path)
                 | 3. namedev_name_device()     |
                 |    → parse /etc/udev/udev.config|
                 |       matching rules:          | 3. delete_node(name)
                 |         LABEL, NUMBER,          |    → unlink("/dev/name")
                 |         TOPOLOGY, REPLACE       |
                 |       → fills struct udevice   |
                 |                               | 4. return
                 | 4. get_major_minor()         |
                 |    → read "dev" attribute      |
                 |       (format "MAJOR:MINOR")    |
                 |                               |
                 | 5. udevdb_add_dev(path,&dev)  |
                 |    → store in TDB (persistent) |
                 |                               |
                 | 6. create_node(&dev)          |
                 |    → mknod("/dev/name", mode, dev_t)|
                 |       mode |= S_IFBLK or S_IFCHR     |
                 |       (uses __KLIBC__ hack if needed)|
                 |                               |
                 v                               v
        +----------------+             +-------------------------+
        |   return retval               |   return retval         |
        +----------------+             +-------------------------+
                                        |
                                        v
                   +-------------------------------------------+
                   |            udevdb_exit()                  |
                   |          → tdb_close()                    |
                   +-------------------------------------------+
                                        |
                                        v
                                   exit(retval)


# Key Components & Data Flow (Detailed)
Environment Variables used:
├── ACTION         → "add" or "remove"
├── DEVPATH        → sysfs path (e.g. /class/usb/host1)
├── SEQNUM         → event sequence number
├── UDEV_TEST      → if set, allow override of paths
├── UDEV_ROOT      → /dev (default)
├── UDEV_DB        → "udev.tdb"
└── UDEV_CONFIG_FILE → "udev.config"

Configuration Files:
├── /etc/udev/udev.config       ← naming rules (example provided)
├── /etc/udev/udev.permissions  ← (exists but not used in code yet)
└── /etc/udev/udev.tdb          ← persistent TDB database

Rule Types in udev.config (parsed by namedev.c):
├── LABEL     → match vendor/model labels
├── NUMBER    → match PCI/USB by bus id, assign numbered names
├── TOPOLOGY  → match USB by port topology (hub.port)
└── REPLACE   → direct KERNEL name override

Database (TDB):
Key   → DEVPATH string (null-terminated)
Value → struct udevice {
          char name[100];
          char owner[30];
          char group[30];
          char type;      // 'b','c','u','p'
          int major, minor;
          mode_t mode;
        }


# Execution Example: USB Camera Inserted
Kernel → hotplug → /sbin/udev usb
   env: ACTION=add
        DEVPATH=/class/usb_device/1234-5678
        BUS=usb, vendor=FUJIFILM

udev main()
 └→ get_dirs() → udev_root="/dev"
 └→ udevdb_init() → open /etc/udev/udev.tdb
 └→ udev_add_device("/class/usb_device/1234-5678", "usb")
      └→ sleep_for_dev() → wait for /sys/.../dev
      └→ get_class_dev()
      └→ namedev_name_device() → matches rule:
           LABEL, BUS="usb", vendor="FUJIFILM", NAME="camera"
           → dev.name = "camera"
      └→ get_major_minor() → reads "dev" → 180:0
      └→ udevdb_add_dev() → store in TDB
      └→ create_node() → mknod("/dev/camera", S_IFCHR|0660, makedev(180,0))


# Removal Example
ACTION=remove → udev_remove_device()
 └→ get_name() → TDB lookup → "camera"
 └→ udevdb_delete_dev()
 └→ unlink("/dev/camera")

# Summary of This 2003 Design (Version 005)
Pure userspace devfs replacement
No udevd daemon — direct hotplug script execution
No rule parser in main binary — namedev_name_device() does it
Persistent database in /etc/udev/udev.tdb (TDB)
Very small codebase (~1500 LOC total)
Only handles class + block devices
Ignores network devices
Waits up to 10 seconds for dev attribute
Supports 4 rule types: LABEL, NUMBER, TOPOLOGY, REPLACE
Uses libsysfs heavily
No permission handling yet (permissions file exists but unused)

