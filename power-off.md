# cmds
ss@pc:~/groot/kernel/systemd$ which poweroff
/usr/sbin/poweroff
ss@pc:~/groot/kernel/systemd$ ls -l /usr/sbin/poweroff
lrwxrwxrwx 1 root root 16 Apr 15 11:32 /usr/sbin/poweroff -> ../bin/systemctl
ss@pc:~/groot/kernel/systemd$ which reboot
/usr/sbin/reboot
ss@pc:~/groot/kernel/systemd$ ls -l /usr/sbin/reboot
lrwxrwxrwx 1 root root 16 Apr 15 11:32 /usr/sbin/reboot -> ../bin/systemctl
ss@pc:~/groot/kernel/systemd$ 


# flow
[ USER RUNS: poweroff ]
         │
         ▼
 1. COMMAND TRANSLATION
   ┌─────────────────────────────────────────────────────────────┐
   │ Symlink /usr/bin/poweroff triggers execution redirect       │
   │ Maps directly internally to: systemctl poweroff             │
   └─────────────────────────────────────────────────────────────┘
         │
         ▼
 2. THE MAIN SYSTEMD PROCESS (PID 1) HANDLES TARGETS
   ┌─────────────────────────────────────────────────────────────┐
   │ Systemd isolates poweroff.target                            │
   │ Pulls in systemd-poweroff.service                           │
   └─────────────────────────────────────────────────────────────┘
         │
         ▼
 3. USER-SPACE SERVICE TEARDOWN
   ┌─────────────────────────────────────────────────────────────┐
   │ Services stop sequentially in reverse order of dependency   │
   │ Network targets close, docker / databases exit cleanly       │
   │ Users are logged out, desktop environments terminate         │
   └─────────────────────────────────────────────────────────────┘
         │
         ▼
 4. REPLACING THE CORE EXEC CONTEXT (THE POINT OF NO RETURN)
   ┌─────────────────────────────────────────────────────────────┐
   │ PID 1 calls execve() on /usr/lib/systemd/systemd-shutdown   │
   │ The main systemd service engine completely drops out        │
   │ systemd-shutdown code (src/core/shutdown.c) is now PID 1     │
   └─────────────────────────────────────────────────────────────┘
         │
         ▼
 5. THE SYSTEMD-SHUTDOWN HARDENING LOOP (src/core/shutdown.c)
         │
         ├──► [A] KILL LINGERING PROCESSES
         │    │ Sends SIGTERM, then SIGKILL to remaining tasks
         │    └──────────────────────────────────────────────────
         │
         ├──► [B] TRIM THE CGROUPS TREE
         │    │ Destroys remaining cgroup containers iteratively
         │    └──────────────────────────────────────────────────
         │
         ├──► [C] STORAGE AND STORAGE LAYERS
         │    │ Detaches Device Mapper (DM) components
         │    │ Closes encrypted LUKS drives / loopback volumes
         │    └──────────────────────────────────────────────────
         │
         └──► [D] VIRTUAL FILE SYSTEM DISK SYNC
              │ Calls sync() loops to flush data buffers to disk
              │ Unmounts file systems (Remounts / as Read-Only)
              └──────────────────────────────────────────────────
         │
         ▼
 6. CUSTOM SHUTDOWN HOOK EXECUTIONS
   ┌─────────────────────────────────────────────────────────────┐
   │ Iterates through scripts inside /usr/lib/systemd/system-shutdown/│
   │ Runs remaining last-second hardware scripts or UPS directives│
   └─────────────────────────────────────────────────────────────┘
         │
         ▼
 7. LINUX KERNEL HANDOFF
   ┌─────────────────────────────────────────────────────────────┐
   │ systemd-shutdown calls the low-level reboot() system call   │
   │ Passes flag: LINUX_REBOOT_CMD_POWER_OFF                     │
   └─────────────────────────────────────────────────────────────┘
         │
         ▼
 8. PHYSICAL HARDWARE STATE CHANGE
   ┌─────────────────────────────────────────────────────────────┐
   │ Linux Kernel stops all remaining CPU functions              │
   │ Issues ACPI command directly to the motherboard             │
   │ [ SYSTEM POWER DROPS TO 0W ]                                │
   └─────────────────────────────────────────────────────────────┘

