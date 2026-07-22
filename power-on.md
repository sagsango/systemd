[ src/core/main.c: DEFINE_MAIN_FUNCTION() ]
                        │
                        ▼
 1. EARLY SYSTEM INITIALIZATION (src/core/main.c)
   ┌─────────────────────────────────────────────────────────────┐
   │ main_prepare(): Sets up early logging, signals, & paths     │
   │ Detects environment (Bare metal, KVM, QEMU, LXC, etc.)      │
   │ Mounts virtual API file systems: /proc, /sys, /dev          │
   └─────────────────────────────────────────────────────────────┘
                        │
                        ▼
 2. MANAGER LOAD & SEEDING (src/core/manager.c)
   ┌─────────────────────────────────────────────────────────────┐
   │ manager_new(): Initializes the central service engine       │
   │ Creates the cgroup root path structure                      │
   │ Parses kernel boot parameters (e.g., systemd.log_level)    │
   └─────────────────────────────────────────────────────────────┘
                        │
                        ▼
 3. LOADING UNIT FILES
   ┌─────────────────────────────────────────────────────────────┐
   │ Looks in: /lib/systemd/system/ and /etc/systemd/system/     │
   │ Parses core target definitions                              │
   │ Generates dependency tree (After=, Requires=, Wants=)       │
   └─────────────────────────────────────────────────────────────┘
                        │
                        ▼
 4. BUILDING THE JOB QUEUE
   ┌─────────────────────────────────────────────────────────────┐
   │ Identifies the default boot target (usually default.target) │
   │ Recursively adds all dependent service jobs to the queue   │
   │ Solves cyclic dependency conflicts, drops invalid actions   │
   └─────────────────────────────────────────────────────────────┘
                        │
                        ▼
 5. THE BOOT TRANSACTION EXECUTION
         │
         ├──► [A] sysinit.target (Critical Early Boot)
         │    │ Mounts /etc/fstab file systems, loads crypto swap
         │    │ Sets up udev (systemd-udevd) to scan/create /dev/ devices
         │    └──────────────────────────────────────────────────
         │
         ├──► [B] basic.target (System Base Setup)
         │    │ Initializes timers, sockets, paths, and firewalls
         │    │ Starts systemd-journald for runtime logging
         │    └──────────────────────────────────────────────────
         │
         └──► [C] main event loop (manager_loop())
              │ Uses epoll() to listen for asynchronous events
              │ Spawns individual processes via fork() & execve()
              └──────────────────────────────────────────────────
         │
         ▼
 6. MULTI-USER / GRAPHICAL TARGET
   ┌─────────────────────────────────────────────────────────────┐
   │ Reaches multi-user.target (Starts SSH, Cron, NetworkManager)│
   │ Reaches graphical.target (Starts Display Manager / GDM / X) │
   └─────────────────────────────────────────────────────────────┘
                        │
                        ▼
            [ BOOT PROCESS COMPLETE ]

