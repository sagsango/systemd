# systemd daemon list:
| Category                          | Service Name                              | Description |
|-----------------------------------|-------------------------------------------|-------------|
| Logging and Journaling            | systemd-journald.service                  | Central logging daemon that collects and stores log data from the kernel, services, and applications in a binary journal format for efficient querying and rotation. |
| Logging and Journaling            | systemd-journal-flush.service             | Flushes journal data from memory to disk periodically to ensure persistence. |
| Logging and Journaling            | systemd-journal-remote.service            | Daemon for forwarding logs to a remote server over the network. |
| Logging and Journaling            | systemd-journal-gatewayd.service          | Provides a web-based interface (HTTP/Syslog) for accessing journal logs remotely. |
| Logging and Journaling            | systemd-journal-upload.service            | Uploads journal logs to a remote server using HTTP(S). |
| Logging and Journaling            | systemd-journald@.service                 | Template for per-user journal instances. |
| Logging and Journaling            | systemd-journal-catalog-update.service    | Updates the journal catalog of message IDs to human-readable descriptions. |
| User and Session Management       | systemd-logind.service                    | Manages user logins, sessions, seats, and power events (e.g., lid close, sleep); handles D-Bus interfaces for user authentication and idle detection. |
| User and Session Management       | systemd-user-sessions.service             | Cleans up stale user runtime directories and sessions on boot. |
| User and Session Management       | user@.service                             | Template for per-user service managers. |
| User and Session Management       | systemd-user@.service                     | Template for user-specific instances. |
| User and Session Management       | systemd-user-runtime-dir@.service         | Creates runtime directories for users. |
| User and Session Management       | dbus-org.freedesktop.login1.service       | D-Bus service for logind interfaces. |
| User and Session Management       | dbus-org.freedesktop.hostname1.service    | D-Bus service for hostnamed interfaces. |
| User and Session Management       | dbus-org.freedesktop.locale1.service      | D-Bus service for localed interfaces. |
| User and Session Management       | dbus-org.freedesktop.timedate1.service    | D-Bus service for timedated interfaces. |
| User and Session Management       | getty@.service                            | Template for virtual console login prompts (TTY getty) on serial or console devices. |
| User and Session Management       | serial-getty@.service                     | Template for serial console logins. |
| User and Session Management       | console-getty.service                     | Getty service for console. |
| User and Session Management       | autovt@.service                           | Template for automatic virtual terminal activation. |
| User and Session Management       | container-getty@.service                  | Template for container console getty. |
| User and Session Management       | debug-shell.service                       | Provides a debug shell on TTY9 during boot. |
| Hardware and Device Management    | systemd-udevd.service                     | Dynamic device management daemon that listens for kernel uevents and manages device nodes in /dev, applying rules for permissions and symlinks. |
| Hardware and Device Management    | systemd-udev-trigger.service              | Triggers uevents for already-present devices during early boot to initialize hardware. |
| Hardware and Device Management    | systemd-udev-settle.service               | Waits for all pending uevents to be processed before proceeding with boot. |
| Hardware and Device Management    | systemd-hwdb.service                      | Updates the hardware database (/etc/udev/hwdb.bin) used by udev for device properties. (Note: Often invoked as systemd-hwdb-update.service) |
| Hardware and Device Management    | systemd-rfkill.service                    | Manages radio frequency (RF) kill switches for Wi-Fi, Bluetooth, etc., blocking/unblocking devices based on hardware switches. |
| Hardware and Device Management    | sockets.target.wants/systemd-udevd-control.socket | Socket for udev control. |
| Hardware and Device Management    | sockets.target.wants/systemd-udevd-kernel.socket | Kernel socket for udev events. |
| Hardware and Device Management    | sockets.target.wants/systemd-udevd-varlink.socket | Varlink socket for udev. |
| Hardware and Device Management    | initrd-udevadm-cleanup-db.service         | Cleans up udev database in initrd. |
| Hardware and Device Management    | kmod-static-nodes.service                 | Creates static device nodes from modules. |
| Hardware and Device Management    | modprobe@.service                         | Template for loading specific kernel modules. |
| Hardware and Device Management    | systemd-udev-load-credentials.service     | Loads credentials for udev. |
| Networking and Resolution         | systemd-networkd.service                  | Lightweight daemon for configuring network interfaces, routes, and addresses via .network files; supports static, DHCP, and VLAN setups. |
| Networking and Resolution         | systemd-networkd-wait-online@.service     | Template to block until network is online for specific interfaces. |
| Networking and Resolution         | systemd-resolved.service                  | Stub DNS resolver that provides name resolution, caching, and DNSSEC validation; integrates with resolv.conf. |
| Networking and Resolution         | systemd-resolved-wait-online.service      | Waits for DNS resolution to be available before proceeding. |
| Time and Host Configuration       | systemd-timesyncd.service                 | Simple NTP client daemon for synchronizing system clock over the network using NTP. |
| Time and Host Configuration       | systemd-timedated.service                 | D-Bus service for querying and changing system time, timezone, and NTP settings. |
| Time and Host Configuration       | systemd-hostnamed.service                 | D-Bus service for querying and changing the system hostname and related machine info. |
| Time and Host Configuration       | systemd-localed.service                   | D-Bus service for querying and changing system locale and internationalization settings. |
| Time and Host Configuration       | systemd-time-wait-sync.service            | Waits for time synchronization during boot. |
| Boot and Filesystem Management    | systemd-remount-fs.service                | Remounts root and other filesystems according to /etc/fstab options during early boot. |
| Boot and Filesystem Management    | systemd-fsck@.service                     | Template service for checking specific filesystems (e.g., for non-root mounts). |
| Boot and Filesystem Management    | systemd-fsck-root.service                 | Performs filesystem checks (fsck) on the root filesystem before mounting. |
| Boot and Filesystem Management    | systemd-growfs@.service                   | Grows (resizes) filesystems during boot if the underlying block device has been expanded. |
| Boot and Filesystem Management    | systemd-cryptsetup@.service               | Template for unlocking and setting up LUKS-encrypted block devices. (Note: Often under cryptsetup.target) |
| Boot and Filesystem Management    | systemd-tmpfiles-setup.service            | Creates, deletes, and adjusts ownership/permissions for volatile files (e.g., /tmp, /var/tmp) based on tmpfiles.d configs. |
| Boot and Filesystem Management    | systemd-tmpfiles-setup-dev.service        | Sets up essential device files in /dev during early boot. |
| Boot and Filesystem Management    | systemd-tmpfiles-clean.service            | Periodically cleans up temporary files based on age and rules. |
| Boot and Filesystem Management    | systemd-tmpfiles-setup-dev-early.service  | Early setup of device files in initrd. |
| Boot and Filesystem Management    | systemd-sysctl.service                    | Applies kernel sysctl settings from sysctl.d configuration files. |
| Boot and Filesystem Management    | systemd-modules-load.service              | Loads kernel modules listed in /etc/modules-load.d during boot. |
| Boot and Filesystem Management    | systemd-random-seed.service               | Saves and loads a random seed to /var/lib/systemd/random-seed for faster entropy initialization on boot. |
| Boot and Filesystem Management    | systemd-machine-id-commit.service         | Commits the machine ID to disk (/etc/machine-id) on first boot or when changed. |
| Boot and Filesystem Management    | initrd-switch-root.service                | Switches from initrd to real root filesystem. |
| Boot and Filesystem Management    | initrd-root-fs.target.wants/systemd-repart.service | Repartitions root in initrd. |
| Boot and Filesystem Management    | ldconfig.service                          | Updates shared library cache. |
| Boot and Filesystem Management    | quotaon-root.service                      | Enables quotas on root filesystem. |
| Boot and Filesystem Management    | quotaon@.service                          | Template for enabling quotas on specific filesystems. |
| Boot and Filesystem Management    | systemd-quotacheck-root.service           | Checks quotas on root. |
| Boot and Filesystem Management    | systemd-quotacheck@.service               | Template for quota checks. |
| Boot and Filesystem Management    | systemd-update-done.service               | Marks boot as complete. |
| Boot and Filesystem Management    | systemd-update-utmp.service               | Updates utmp/wtmp with boot events. |
| Boot and Filesystem Management    | systemd-vconsole-setup.service            | Sets up virtual console fonts and keymaps. |
| Boot and Filesystem Management    | systemd-volatile-root.service             | Sets up volatile root filesystem. |
| Boot and Filesystem Management    | systemd-validatefs@.service               | Validates filesystem integrity. |
| Boot and Filesystem Management    | systemd-mountfsd.service                  | Filesystem mounting daemon. |
| Boot and Filesystem Management    | systemd-loop@.service                     | Template for loop device management. |
| Power and Shutdown Management     | systemd-suspend.service                   | Handles system suspend-to-RAM (S3 sleep) by freezing processes and writing state to disk. |
| Power and Shutdown Management     | systemd-hibernate.service                 | Handles full hibernation by dumping memory to disk (swap) and powering off. |
| Power and Shutdown Management     | systemd-hybrid-sleep.service              | Combines suspend and hibernate: suspends immediately but dumps to disk for safety. |
| Power and Shutdown Management     | systemd-suspend-then-hibernate.service    | Suspends first, then hibernates if suspend lasts too long (e.g., low battery). |
| Power and Shutdown Management     | systemd-backlight@.service                | Saves and restores backlight brightness for specific devices (e.g., laptop screen). |
| Power and Shutdown Management     | systemd-pstore.service                    | Archives platform persistent storage (e.g., EFI variables) to the journal on shutdown. |
| Power and Shutdown Management     | systemd-halt.service                      | Halts the system. |
| Power and Shutdown Management     | systemd-poweroff.service                  | Powers off the system. |
| Power and Shutdown Management     | systemd-reboot.service                    | Reboots the system. |
| Power and Shutdown Management     | systemd-kexec.service                     | Performs kexec reboot. |
| Power and Shutdown Management     | systemd-hibernate-clear.service           | Clears hibernation state. |
| System Initialization and Maintenance | systemd-sysusers.service               | Creates system users and groups defined in sysusers.d configuration files during boot. |
| System Initialization and Maintenance | systemd-firstboot.service                | Runs one-time setup tasks (e.g., generating SSH keys) on the first boot after installation. |
| System Initialization and Maintenance | systemd-update-utmp-runlevel.service    | Logs runlevel changes (legacy compatibility) to utmp. |
| System Initialization and Maintenance | systemd-binfmt.service                   | Sets up support for additional binary formats (e.g., via QEMU binfmt_misc for emulation). |
| System Initialization and Maintenance | systemd-coredump@.service                | Template for handling core dumps from crashed processes, storing them compressed. |
| System Initialization and Maintenance | emergency.service                        | Emergency shell mode. |
| System Initialization and Maintenance | rescue.service                           | Rescue mode shell. |
| System Initialization and Maintenance | initrd-cleanup.service                   | Cleans up initrd environment. |
| System Initialization and Maintenance | systemd-bless-boot.service               | Blesses boot partition for EFI. |
| System Initialization and Maintenance | systemd-bootctl@.service                 | Manages systemd-boot loader. |
| System Initialization and Maintenance | systemd-sysupdate.service                | Updates system extensions. |
| Virtualization and Containers     | systemd-machined.service                  | Manages virtual machines and containers, providing D-Bus APIs for import/export and state tracking. |
| Virtualization and Containers     | systemd-nspawn@.service                   | Template for running containers using Linux namespaces and cgroups (lightweight alternative to Docker). |
| Virtualization and Containers     | capsule@.service                          | Template for capsule management (UKI). |
| Virtualization and Containers     | systemd-vmspawn@.service                  | Template for VM spawning. |
| Virtualization and Containers     | dbus-org.freedesktop.machine1.service     | D-Bus for machined. |
| Virtualization and Containers     | dbus-org.freedesktop.portable1.service    | D-Bus for portable services. |
| Security and Credentials          | systemd-creds@.service                    | Manages credentials. |
| Security and Credentials          | sockets.target.wants/systemd-creds.socket | Socket for creds. |
| Security and Credentials          | systemd-userdb-load-credentials.service   | Loads user credentials. |
| Security and Credentials          | systemd-userdbd.service                   | User database daemon. |
| Out of Memory Management          | systemd-oomd.service                      | Out-of-memory (OOM) killer daemon that monitors memory usage and kills processes to prevent OOM conditions. |
| Home Directory Management         | systemd-homed.service                     | Manages portable home directories with encryption and portability. |
| Network Name Resolution           | dbus-org.freedesktop.resolve1.service     | D-Bus for resolved (implied). |
| Portable Services                 | systemd-portabled.service                 | Manages portable services and applications. |
| dbus-org.freedesktop.import1.service | D-Bus for importd. |
| Extensions and Updates            | systemd-sysext@.service                   | Template for system extensions. |
| Extensions and Updates            | sockets.target.wants/systemd-sysext.socket | Socket for sysext. |
| Extensions and Updates            | systemd-importd.service                   | Imports portable data. |
| Extensions and Updates            | sockets.target.wants/systemd-importd.socket | Socket for importd. |
| TPM and PCR Management            | systemd-tpm2-setup.service                | Sets up TPM2 device. |
| TPM and PCR Management            | systemd-tpm2-setup-early.service          | Early TPM2 setup in initrd. |
| TPM and PCR Management            | systemd-tpm2-clear.service                | Clears TPM2. |
| TPM and PCR Management            | systemd-pcrmachine.service                | Manages PCR for machine ID. |
| TPM and PCR Management            | systemd-pcrphase.service                  | Handles PCR phases during boot. |
| TPM and PCR Management            | systemd-pcrphase-initrd.service           | PCR phase in initrd. |
| TPM and PCR Management            | systemd-pcrphase-sysinit.service          | PCR phase in sysinit. |
| TPM and PCR Management            | systemd-pcrfs@.service                    | PCR for filesystem. |
| TPM and PCR Management            | systemd-pcrlock@.service                  | PCR lock management. |
| TPM and PCR Management            | sockets.target.wants/systemd-pcrlock.socket | Socket for pcrlock. |
| TPM and PCR Management            | sockets.target.wants/systemd-pcrextend.socket | Socket for pcrextend. |
| TPM and PCR Management            | systemd-pcrextend@.service                | Extends PCR measurements. |
| Factory Reset                     | systemd-factory-reset@.service            | Template for factory reset operations. |
| Factory Reset                     | sockets.target.wants/systemd-factory-reset.socket | Socket for factory reset. |
| Factory Reset                     | factory-reset.target.wants/systemd-factory-reset-request.service | Requests factory reset. |
| Factory Reset                     | factory-reset.target.wants/systemd-pcrphase-factory-reset.service | PCR phase for factory reset. |
| Storage Target Mode               | storage-target-mode.target.wants/systemd-pcrphase-storage-target-mode.service | PCR for storage target mode. |
| Other Core Services               | systemd-battery-check.service             | (Optional) Checks battery status and inhibits suspend if critically low. |
| Other Core Services               | dbus.service                              | System message bus (though not always listed as .service, it's core). |
| Other Core Services               | rescue.service                            | Rescue shell (already listed). |
| Resource Management               | systemd-nsresourced.service               | Namespaces resource management. |
| Resource Management               | systemd-storagetm.service                 | Storage target mode daemon. |
| Boot Loader and Random Seed       | sysinit.target.wants/systemd-boot-random-seed.service | Generates random seed for boot. |
| Boot Loader and Random Seed       | sockets.target.wants/systemd-bootctl.socket | Socket for bootctl. |
| Password Management               | systemd-ask-password@.service             | Template for asking passwords (e.g., for cryptsetup). |
| Password Management               | systemd-ask-password-console.service      | Console password prompter. |
| Password Management               | systemd-ask-password-wall.service         | Wall (broadcast) password prompter. |
| Password Management               | sysinit.target.wants/systemd-ask-password-console.path | Path trigger for ask-password. |
| Password Management               | multi-user.target.wants/systemd-ask-password-wall.path | Path for wall passwords. |
| Password Management               | sockets.target.wants/systemd-ask-password.socket | Socket for ask-password. |
| Core Dump                         | sockets.target.wants/systemd-coredump.socket | Socket for core dump handling. |
| Journal Dev Log                   | sockets.target.wants/systemd-journald-dev-log.socket | Dev log socket for journald. |
| Journal Socket                    | sockets.target.wants/systemd-journald.socket | Socket activation for journald. |
| Logind Varlink                    | sockets.target.wants/systemd-logind-varlink.socket | Varlink socket for logind. |
| Machined Socket                   | sockets.target.wants/systemd-machined.socket | Socket for machined. |
| Hostnamed Socket                  | sockets.target.wants/systemd-hostnamed.socket | Socket for hostnamed. |
| Sysinit Targets (Mounts)          | sysinit.target.wants/dev-hugepages.mount  | Mounts /dev/hugepages. |
| Sysinit Targets (Mounts)          | sysinit.target.wants/dev-mqueue.mount     | Mounts /dev/mqueue. |
| Sysinit Targets (Mounts)          | sysinit.target.wants/sys-fs-fuse-connections.mount | Mounts FUSE connections. |
| Sysinit Targets (Mounts)          | sysinit.target.wants/sys-kernel-config.mount | Mounts kernel config. |
| Sysinit Targets (Mounts)          | sysinit.target.wants/sys-kernel-debug.mount | Mounts kernel debug. |
| Sysinit Targets (Mounts)          | sysinit.target.wants/sys-kernel-tracing.mount | Mounts kernel tracing. |
| Sysinit Targets (Mounts)          | sysinit.target.wants/proc-sys-fs-binfmt_misc.automount | Automounts binfmt_misc. |
| Sysinit Targets (Mounts)          | local-fs.target.wants/tmp.mount           | Mounts /tmp. |
| Sysinit Targets (Mounts)          | machines.target.wants/var-lib-machines.mount | Mounts /var/lib/machines. |
| Sysinit Targets (Mounts)          | remote-fs.target.wants/var-lib-machines.mount | Remote FS mount for machines. |
| Cryptsetup and Integrity          | sysinit.target.wants/cryptsetup.target    | Target for cryptsetup services. |
| Cryptsetup and Integrity          | sysinit.target.wants/integritysetup.target | Target for integritysetup. |
| Cryptsetup and Integrity          | sysinit.target.wants/veritysetup.target   | Target for veritysetup. |
| Cryptsetup and Integrity          | initrd-root-device.target.wants/remote-cryptsetup.target | Remote cryptsetup in initrd. |
| Cryptsetup and Integrity          | initrd-root-device.target.wants/remote-integritysetup.target | Remote integrity in initrd. |
| Cryptsetup and Integrity          | initrd-root-device.target.wants/remote-veritysetup.target | Remote verity in initrd. |
| Repart and Imports                | sysinit.target.wants/imports.target       | Target for imports. |
| Multi-User Targets                | multi-user.target.wants/getty.target      | Target for getty services. |
| Multi-User Targets                | multi-user.target.wants/systemd-logind.service | Enables logind in multi-user. |
| Multi-User Targets                | multi-user.target.wants/systemd-user-sessions.service | Enables user sessions cleanup. |
| Sysinit Targets                   | sysinit.target.wants/systemd-update-utmp.service | Enables utmp update. |

# Usage Notes:
# - This giant table includes all core .service units from the systemd package (as of Arch Linux 258.2-2, November 2025), plus previous ones. Some entries are targets or paths but included if they reference services.
# - Categories are grouped logically; some services fit multiple but placed in primary.
# - Descriptions are based on official systemd documentation and man pages.
# - Distro-specific services (e.g., NetworkManager.service, bluetooth.service) are omitted to focus on core systemd ones.
# - To add more: Insert rows in | Category | Service Name | Description | format.
# - For even larger, add columns like | Enabled by Default | Dependencies |.
# - Copy-paste into a Markdown file for rendering.
