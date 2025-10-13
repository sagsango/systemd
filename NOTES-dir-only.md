/Users/sagarsingh/groot/kernel/systemd
.
├── catalog     : XXX - define structured log messages for systemd-journald
├── coccinelle  : XXX - GitHub and citation tools to reference this project in academic papers
├── docs        : XXX - documentation and its conf
│   ├── _data
│   ├── _includes
│   ├── _layouts
│   ├── assets
│   ├── fonts
│   ├── sysvinit
│   └── var-log
├── factory     : XXX - default configs
│   ├── etc
│   │   └── pam.d
│   └── templates
├── hwdb.d      : XXX - Hardware database rules for udev.
├── LICENSES
├── man         : XXX - man pages
│   └── rules
├── mime    : XXX - MIME type definitions — used to integrate systemd tools with desktop environments (e.g., .service files recognized by GUI tools).
├── mkosi   : XXX - how systemd integrates with image building, booting, and containers.
│   ├── keydev.repart
│   ├── mkosi.conf.d
│   │   ├── arch
│   │   │   └── mkosi.conf.d
│   │   ├── centos
│   │   ├── centos-fedora
│   │   │   └── mkosi.conf.d
│   │   ├── debian
│   │   │   └── mkosi.conf.d
│   │   ├── debian-ubuntu
│   │   │   └── mkosi.conf.d
│   │   ├── fedora
│   │   │   └── mkosi.conf.d
│   │   ├── opensuse
│   │   │   └── mkosi.conf.d
│   │   └── ubuntu
│   │       └── mkosi.conf.d
│   ├── mkosi.coverage
│   ├── mkosi.credentials
│   ├── mkosi.extra
│   │   ├── etc
│   │   │   └── iscsi
│   │   ├── root
│   │   └── usr
│   │       ├── lib
│   │       │   ├── sysctl.d
│   │       │   ├── systemd
│   │       │   │   └── system
│   │       │   │       └── user@.service.d
│   │       │   └── tmpfiles.d
│   │       └── share
│   │           └── dbus-1
│   │               └── system.d
│   ├── mkosi.extra.common
│   │   ├── etc
│   │   └── usr
│   │       └── lib
│   │           └── systemd
│   │               ├── coredump.conf.d
│   │               ├── journald.conf.d
│   │               ├── system
│   │               └── system-preset
│   ├── mkosi.images
│   │   ├── build
│   │   │   └── mkosi.conf.d
│   │   │       ├── arch
│   │   │       ├── centos
│   │   │       │   └── mkosi.conf.d
│   │   │       ├── centos-fedora
│   │   │       ├── debian-ubuntu
│   │   │       ├── fedora
│   │   │       └── opensuse
│   │   ├── exitrd
│   │   │   ├── mkosi.conf.d
│   │   │   └── mkosi.extra
│   │   ├── initrd
│   │   │   ├── mkosi.conf.d
│   │   │   └── mkosi.extra
│   │   │       └── usr
│   │   │           └── lib
│   │   │               ├── encrypted-var.repart.d
│   │   │               └── systemd
│   │   │                   └── system
│   │   ├── minimal-0
│   │   │   └── mkosi.extra
│   │   │       ├── opt
│   │   │       └── usr
│   │   │           └── lib
│   │   │               └── systemd
│   │   │                   └── system
│   │   ├── minimal-1
│   │   │   └── mkosi.extra
│   │   │       ├── opt
│   │   │       └── usr
│   │   │           └── lib
│   │   │               └── systemd
│   │   │                   └── system
│   │   └── minimal-base
│   │       ├── mkosi.conf.d
│   │       └── mkosi.extra
│   │           └── etc
│   ├── mkosi.repart
│   ├── mkosi.sanitizers
│   │   ├── mkosi.conf.d
│   │   └── mkosi.extra
│   │       └── usr
│   │           └── lib
│   │               └── systemd
│   │                   ├── system
│   │                   │   ├── iscsi-init.service.d
│   │                   │   ├── service.d
│   │                   │   ├── systemd-coredump@.service.d
│   │                   │   └── systemd-journald.service.d
│   │                   └── system.conf.d
│   ├── mkosi.tools.conf
│   │   └── mkosi.conf.d
│   │       └── ubuntu
│   │           └── mkosi.conf.d
│   └── mkosi.uki-profiles
├── modprobe.d  : XXX - Default kernel module load configuration snippets — installed to /usr/lib/modprobe.d
├── network     : XXX - Default configurations for systemd-networkd (network interface manager).
├── po
│   └── its
├── presets     : XXX - Defines unit enablement defaults (e.g., which services are enabled by default on first boot).
├── profile.d   : XXX - Default shell environment scripts — affect environment variables, similar to /etc/profile.d.
├── rules.d     : XXX - udev rules — define how devices are initialized when detected by the kernel.
├── shell-completion    : XXX - Shell completion scripts for bash, zsh, and fish — auto-complete systemd commands and units.
│   ├── bash
│   └── zsh
├── src     : XXX - C code for systemd components
│   ├── ac-power    : XXX - Implementation of AC power detection and management utilities.
│   ├── analyze     : XXX - Source for the systemd-analyze tool, used for examining systemd timings, dependencies, and security.
│   ├── ask-password    : XXX - Code for password prompting mechanisms, used in boot processes like cryptsetup.
│   ├── backlight   : XXX - Backlight control utilities for display brightness management.
│   ├── basic   : XXX - Core primitives and utilities used across all user-space components of systemd
│   ├── battery-check   : XXX - Battery status monitoring and alerting tools.
│   ├── binfmt  : XXX - Support for binfmt_misc kernel module registration.
│   ├── bless-boot  : XXX - Utilities for "blessing" boot entries in EFI firmware.
│   ├── boot : XXX - Boot process-related code, including EFI stubs. 
│   │   ├── hwids
│   │   └── proto
│   ├── bootctl : XXX - Source for the bootctl tool to manage systemd-boot.
│   ├── busctl  : XXX - Implementation of the busctl D-Bus introspection and message-sending tool.
│   ├── cgls    : XXX - Code for the cgls tool to visualize cgroup hierarchies.
│   ├── cgtop   : XXX - Source for the cgtop tool to monitor cgroup resource usage in real-time.
│   ├── core    : XXX - Main logic for the systemd service manager (PID 1), including unit management and process supervision
│   │   └── bpf
│   │       ├── restrict-fs
│   │       ├── restrict-ifaces
│   │       └── socket-bind
│   ├── coredump    : XXX - Core dump collection and handling daemon
│   ├── coverage    : XXX - Tools for code coverage analysis during testing.
│   ├── creds   : XXX - Credential storage and retrieval utilities.
│   ├── cryptenroll : XXX - Source for the cryptenroll tool to manage cryptographic keys for LUKS volumes. 
│   ├── cryptsetup  : XXX - Integration with cryptsetup for encrypted volume management.
│   │   └── cryptsetup-tokens
│   ├── debug-generator : XXX - Generator for debug-related systemd units.
│   ├── delta   : XXX - Utilities for computing and applying deltas in system updates.
│   ├── detect-virt : XXX - Virtualization detection logic.
│   ├── dissect : XXX - Image dissection tools for analyzing disk images in portable services.
│   ├── environment-d-generator : XXX - Generator for processing environment.d configuration files.
│   ├── escape  : XXX - String escaping and unescaping utilities.
│   ├── factory-reset   : XXX - Factory reset functionality for embedded systems.
│   ├── firstboot   : XXX - First-boot setup and configuration tools.
│   ├── fsck    : XXX - Integration with fsck for filesystem checks during boot.
│   ├── fstab-generator : XXX - Generator that creates mount and swap units from /etc/fstab.
│   ├── fundamental : XXX - Lowest-level primitives used by all code, including EFI and user-space.
│   ├── fuzz    : XXX - Fuzz testing harnesses for various components.
│   ├── getty-generator : XXX - Generator for configuring getty instances on serial consoles.
│   ├── gpt-auto-generator  : XXX - Generator for automatic mounting of GPT-partitioned filesystems.
│   ├── growfs  : XXX - Tool for automatically growing filesystems on first boot.
│   ├── hibernate-resume    : XXX - Hook for resuming from hibernation.
│   ├── home    : XXX - Implementation of systemd-homed for dynamic user home directories.
│   ├── hostname    : XXX - Hostname resolution and setting utilities.
│   ├── hwdb    : XXX - Hardware database (hwdb) for udev.
│   ├── id128   : XXX - 128-bit ID generation and handling utilities.
│   ├── import  : XXX - Tools for importing disk images and qcow2 files.
│   ├── include
│   │   ├── override
│   │   │   ├── linux
│   │   │   ├── net
│   │   │   ├── netinet
│   │   │   └── sys
│   │   └── uapi
│   │       └── linux
│   │           ├── can
│   │           ├── hdlc
│   │           ├── netfilter
│   │           ├── netfilter_ipv4
│   │           └── sched
│   ├── integritysetup  : XXX - Support for dm-integrity device-mapper targets.
│   ├── journal : XXX - Logging system (systemd-journald) and related tools.
│   ├── journal-remote  : XXX, TODO - Remote journaling capabilities for receiving logs over the network.
│   ├── kernel-install  : XXX - Hooks and tools for kernel package installation.
│   ├── keyutil : XXX - Key utility functions for cryptographic operations.
│   ├── libc    : Wrappers and polyfills for libc functions.
│   ├── libsystemd  : XXX - Shared library libsystemd for client-side systemd interactions.
│   │   ├── sd-bus
│   │   ├── sd-daemon
│   │   ├── sd-device
│   │   ├── sd-event
│   │   ├── sd-hwdb
│   │   ├── sd-id128
│   │   ├── sd-journal
│   │   ├── sd-json
│   │   ├── sd-login
│   │   ├── sd-netlink
│   │   ├── sd-network
│   │   ├── sd-path
│   │   ├── sd-resolve
│   │   └── sd-varlink
│   ├── libsystemd-network  : XXX - Networking library for systemd-networkd.
│   ├── libudev : XXX, TODO - Userspace device management library.
│   ├── locale  : XXX - Locale configuration tools.
│   ├── login   : XXX - User login management, including pam_systemd.
│   ├── machine : XXX - Machine lifecycle management utilities.
│   ├── machine-id-setup    : XXX - Setup for generating machine IDs.
│   ├── measure : XXX - Secure boot measurement tools.
│   ├── modules-load    : XXX, TODO - Early module loading service.
│   ├── mount   : XXX - Mount point management utilities.
│   ├── mountfsd    : XXX - Daemon for handling mount filesystem operations.
│   ├── network : XXX - Network configuration daemon (systemd-networkd)
│   │   ├── bpf
│   │   │   └── sysctl-monitor
│   │   ├── generator
│   │   ├── netdev
│   │   ├── tc
│   │   └── wait-online
│   ├── notify  : XXX - Process notification mechanisms (sd_notify).
│   ├── nspawn  : XXX - Container and VM management (systemd-nspawn).
│   ├── nsresourced : XXX - Namespace resource control daemon.
│   │   └── bpf
│   │       └── userns-restrict
│   ├── nss-myhostnamea : XXX - NSS module for resolving the local hostname.
│   ├── nss-mymachines  : XXX - NSS module for resolving machine names in local networks.
│   ├── nss-resolve : XXX - NSS module for DNS resolution via systemd-resolved.
│   ├── nss-systemd : XXX - NSS module for user/group resolution via systemd.
│   ├── oom : XXX, TODO - Out-of-memory (OOM) killer integration.
│   ├── path    : XXX - Path unit monitoring implementation.
│   ├── pcrextend  : XXX - PCR (Platform Configuration Register) extend utilities for TPM 
│   ├── pcrlock : XXX - PCR-based locking mechanisms.
│   │   └── pcrlock.d   
│   │       ├── 400-secureboot-separator.pcrlock.d
│   │       ├── 500-separator.pcrlock.d
│   │       └── 700-action-efi-exit-boot-services.pcrlock.d
│   ├── portable    : XXX - Portable service image management.
│   │   └── profile
│   │       ├── default
│   │       ├── nonetwork
│   │       ├── strict
│   │       └── trusted
│   ├── pstore  : XXX - Persistent storage access for EFI variables.
│   ├── ptyfwd  : XXX - Pseudo-terminal forwarding utilities.
│   ├── quotacheck  : XXX - Filesystem quota checking integration.
│   ├── random-seed : XXX - Random seed generation and storage service.
│   ├── rc-local-generator  : XXX - Generator for legacy /etc/rc.local compatibility.
│   ├── remount-fs  : XXX - Filesystem remounting service during boot.
│   ├── repart  : XXX - Disk repartitioning tool (systemd-repart). 
│   │   └── definitions
│   │       ├── confext.repart.d
│   │       ├── portable.repart.d
│   │       └── sysext.repart.d
│   ├── reply-password  : XXX - Password reply handling for agents.
│   ├── resolve : XXX - DNS resolver daemon (systemd-resolved).
│   ├── rfkill  : XXX - RF kill switch handling service.
│   ├── rpm : XXX, TODO - RPM packaging specifications and helpers.
│   ├── run : XXX - Runtime directory management.
│   ├── run-generator   : XXX - Generator for runtime units.
│   ├── sbsign  : XXX, TODO - Signing utilities for secure boot (sb-sign).
│   ├── shared  : XXX - Shared utilities library (libsystemd-shared).
│   ├── shutdown    : XXX, TODO - System shutdown and reboot logic.
│   ├── sleep   : XXX - Suspend and sleep state management.
│   ├── socket-activate  : XXX - Socket-based service activation.
│   ├── socket-proxy    : XXX - Socket proxying utilities.
│   ├── ssh-generator   : XXX - Generator for SSH keys in nspawn containers.
│   ├── stdio-bridge    : XXX - Stdio bridging for forwarded streams.
│   ├── storagetm   : XXX - Storage temperature monitoring.
│   ├── sulogin-shell   : XXX - Single-user login shell implementation.
│   ├── sysctl  : XXX - Sysctl parameter setting service.
│   ├── sysext  : XXX - System extension image management.
│   ├── system-update-generator  : XXX - Generator for system update units.
│   ├── systemctl   : XXX - Implementation of the systemctl management tool.
│   ├── systemd : XXX, TODO - Core PID 1 (init) implementation.
│   ├── sysupdate   : XXX - System update tool for A/B updates.
│   ├── sysusers    : XXX - User and group creation from spec files (systemd-sysusers).
│   ├── sysv-generator  : XXX - Generator for SysV init script compatibility.
│   ├── test
│   ├── timedate
│   ├── timesync
│   ├── tmpfiles
│   ├── tpm2-setup
│   ├── tty-ask-password-agent
│   ├── udev    : XXX, TODO - Device management daemon and tools (udev)
│   │   ├── ata_id
│   │   ├── cdrom_id
│   │   ├── dmi_memory_id
│   │   ├── fido_id
│   │   ├── iocost
│   │   ├── mtd_probe
│   │   ├── net
│   │   ├── scsi_id
│   │   └── v4l_id
│   ├── ukify   : XXX - Unified Kernel Image (UKI) creation tool.
│   │   └── test
│   ├── update-done : XXX - Update completion marking.
│   ├── update-utmp : XXX - Utmp updates for login sessions.
│   ├── user-sessions   : XXX - User session tracking and management.
│   ├── userdb  : XXX, TODO - User database utilities.
│   ├── validatefs  : XXX, TODO - Filesystem validation tools.
│   ├── varlinkctl  : XXX - Varlink interface control tool.
│   ├── vconsole    : XXX - Virtual console setup.
│   ├── veritysetup : XXX, TODO - dm-verity setup for verified boot.
│   ├── version : XXX - Version information and git utilities.
│   ├── vmspawn : XXX, TODO - Virtual machine spawning utilities.
│   ├── volatile-root   : XXX, TODO - Support for volatile / root filesystem.
│   ├── vpick
│   └── xdg-autostart-generator
├── sysctl.d    : XXX - Default sysctl configuration — kernel parameter settings applied at boot via systemd-sysctl.
├── sysusers.d  : XXX - Configuration for creating system users/groups at boot (systemd-sysusers).
├── test    : XXX - Automated test suite — unit tests, integration tests, and QEMU-based image tests.
│   ├── auxv
│   ├── dmidecode-dumps
│   ├── fuzz
│   │   ├── fuzz-bootspec
│   │   ├── fuzz-bus-match
│   │   ├── fuzz-bus-message
│   │   ├── fuzz-calendarspec
│   │   ├── fuzz-catalog
│   │   ├── fuzz-compress
│   │   ├── fuzz-dhcp-client
│   │   ├── fuzz-dhcp-server
│   │   ├── fuzz-dhcp-server-relay
│   │   ├── fuzz-dhcp6-client
│   │   ├── fuzz-dns-packet
│   │   ├── fuzz-env-file
│   │   ├── fuzz-etc-hosts
│   │   ├── fuzz-execute-serialize
│   │   ├── fuzz-fido-id-desc
│   │   ├── fuzz-journal-remote
│   │   ├── fuzz-journald-audit
│   │   ├── fuzz-journald-kmsg
│   │   ├── fuzz-journald-native-fd
│   │   ├── fuzz-journald-stream
│   │   ├── fuzz-journald-syslog
│   │   ├── fuzz-json
│   │   ├── fuzz-link-parser
│   │   ├── fuzz-lldp-rx
│   │   ├── fuzz-manager-serialize
│   │   ├── fuzz-ndisc-rs
│   │   ├── fuzz-netdev-parser
│   │   ├── fuzz-network-parser
│   │   ├── fuzz-nspawn-oci
│   │   ├── fuzz-nspawn-settings
│   │   ├── fuzz-resource-record
│   │   ├── fuzz-systemctl-parse-argv
│   │   ├── fuzz-udev-database
│   │   ├── fuzz-udev-rules
│   │   ├── fuzz-unit-file
│   │   ├── fuzz-varlink
│   │   ├── fuzz-varlink-idl
│   │   └── fuzz-xdg-desktop
│   ├── hwdb.d
│   ├── integration-tests
│   │   ├── standalone
│   │   │   └── integration-tests -> ..
│   │   ├── TEST-01-BASIC
│   │   ├── TEST-02-UNITTESTS
│   │   ├── TEST-03-JOBS
│   │   │   └── TEST-03-JOBS.units
│   │   ├── TEST-04-JOURNAL
│   │   │   └── TEST-04-JOURNAL.units
│   │   ├── TEST-05-RLIMITS
│   │   ├── TEST-06-SELINUX
│   │   │   └── TEST-06-SELINUX.units
│   │   ├── TEST-07-PID1
│   │   │   └── TEST-07-PID1.units
│   │   │       └── local-fs.target.wants
│   │   ├── TEST-08-INITRD
│   │   ├── TEST-09-REBOOT
│   │   ├── TEST-13-NSPAWN
│   │   ├── TEST-15-DROPIN
│   │   ├── TEST-16-EXTEND-TIMEOUT
│   │   │   └── TEST-16-EXTEND-TIMEOUT.units
│   │   ├── TEST-17-UDEV
│   │   ├── TEST-18-FAILUREACTION
│   │   ├── TEST-19-CGROUP
│   │   ├── TEST-21-DFUZZER
│   │   ├── TEST-22-TMPFILES
│   │   ├── TEST-23-UNIT-FILE
│   │   │   └── TEST-23-UNIT-FILE.units
│   │   ├── TEST-24-CRYPTSETUP
│   │   ├── TEST-25-IMPORT
│   │   ├── TEST-26-SYSTEMCTL
│   │   ├── TEST-29-PORTABLE
│   │   ├── TEST-30-ONCLOCKCHANGE
│   │   │   └── TEST-30-ONCLOCKCHANGE.units
│   │   │       └── systemd-timedated.service.d
│   │   ├── TEST-31-DEVICE-ENUMERATION
│   │   ├── TEST-32-OOMPOLICY
│   │   ├── TEST-34-DYNAMICUSERMIGRATE
│   │   ├── TEST-35-LOGIN
│   │   ├── TEST-36-NUMAPOLICY
│   │   ├── TEST-38-FREEZER
│   │   ├── TEST-43-PRIVATEUSER-UNPRIV
│   │   ├── TEST-44-LOG-NAMESPACE
│   │   ├── TEST-45-TIMEDATE
│   │   ├── TEST-46-HOMED
│   │   ├── TEST-50-DISSECT
│   │   ├── TEST-52-HONORFIRSTSHUTDOWN
│   │   │   └── TEST-52-HONORFIRSTSHUTDOWN.units
│   │   ├── TEST-53-ISSUE-16347
│   │   ├── TEST-54-CREDS
│   │   ├── TEST-55-OOMD
│   │   ├── TEST-58-REPART
│   │   ├── TEST-59-RELOADING-RESTART
│   │   ├── TEST-60-MOUNT-RATELIMIT
│   │   ├── TEST-62-RESTRICT-IFACES
│   │   ├── TEST-63-PATH
│   │   │   └── TEST-63-PATH.units
│   │   ├── TEST-64-UDEV-STORAGE
│   │   ├── TEST-65-ANALYZE
│   │   ├── TEST-66-DEVICE-ISOLATION
│   │   ├── TEST-67-INTEGRITY
│   │   ├── TEST-68-PROPAGATE-EXIT-STATUS
│   │   ├── TEST-69-SHUTDOWN
│   │   ├── TEST-70-TPM2
│   │   ├── TEST-71-HOSTNAME
│   │   ├── TEST-72-SYSUPDATE
│   │   ├── TEST-73-LOCALE
│   │   ├── TEST-74-AUX-UTILS
│   │   │   └── TEST-74-AUX-UTILS.units
│   │   ├── TEST-75-RESOLVED
│   │   ├── TEST-76-SYSCTL
│   │   ├── TEST-78-SIGQUEUE
│   │   ├── TEST-79-MEMPRESS
│   │   ├── TEST-80-NOTIFYACCESS
│   │   │   └── TEST-80-NOTIFYACCESS.units
│   │   ├── TEST-81-GENERATORS
│   │   ├── TEST-82-SOFTREBOOT
│   │   ├── TEST-83-BTRFS
│   │   ├── TEST-84-STORAGETM
│   │   ├── TEST-85-NETWORK
│   │   ├── TEST-86-MULTI-PROFILE-UKI
│   │   ├── TEST-87-AUX-UTILS-VM
│   │   └── TEST-88-UPGRADE
│   ├── journal-data
│   ├── knot-data
│   │   └── zones
│   ├── test-bcd
│   ├── test-execute
│   ├── test-fstab-generator
│   │   ├── test-01-dev-nfs.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-02-dhcp.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-03-dhcp6.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-04-nfs.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-05-nfs4.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-06-ipv4.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-07-ipv6.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-08-implicit-nfs.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-09-cifs.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-10-iscsi.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-11-live.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-12-dev-sdx.expected
│   │   │   ├── initrd-root-device.target.d
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-13-label.expected
│   │   │   ├── initrd-root-device.target.d
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-14-uuid.expected
│   │   │   ├── initrd-root-device.target.d
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-15-partuuid.expected
│   │   │   ├── initrd-root-device.target.d
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-16-tmpfs.expected
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-17-initrd-sysroot.fstab.expected
│   │   │   ├── initrd-fs.target.requires
│   │   │   ├── initrd-root-device.target.d
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   └── initrd-usr-fs.target.requires
│   │   ├── test-17-initrd-sysroot.fstab.expected.sysroot
│   │   │   ├── local-fs.target.requires
│   │   │   └── local-fs.target.wants
│   │   ├── test-18-options.fstab.expected
│   │   │   ├── foo.service.requires
│   │   │   ├── foo.service.wants
│   │   │   ├── initrd-root-device.target.d
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   ├── local-fs.target.d
│   │   │   ├── local-fs.target.requires
│   │   │   ├── local-fs.target.wants
│   │   │   ├── mnt-growfs.mount.wants
│   │   │   └── mnt-mkfs.mount.requires
│   │   ├── test-18-options.fstab.expected.sysroot
│   │   │   ├── foo.service.requires
│   │   │   ├── foo.service.wants
│   │   │   ├── local-fs.target.d
│   │   │   ├── local-fs.target.requires
│   │   │   ├── local-fs.target.wants
│   │   │   ├── mnt-growfs.mount.wants
│   │   │   └── mnt-mkfs.mount.requires
│   │   ├── test-19-mounts-from-cmdline.expected
│   │   │   ├── initrd-fs.target.requires
│   │   │   ├── initrd-root-device.target.d
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   ├── local-fs.target.requires
│   │   │   └── remote-fs.target.requires
│   │   ├── test-19-mounts-from-cmdline.expected.sysroot
│   │   │   └── local-fs.target.requires
│   │   ├── test-20-swap-from-cmdline.expected
│   │   │   ├── dev-sdy2.swap.requires
│   │   │   ├── dev-sdy3.swap.requires
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   ├── swap.target.requires
│   │   │   └── swap.target.wants
│   │   ├── test-20-swap-from-cmdline.expected.container
│   │   │   └── initrd-usr-fs.target.requires
│   │   └── test-20-swap-from-cmdline.expected.sysroot
│   │       └── swap.target.requires
│   ├── test-journals
│   │   ├── corrupted
│   │   └── no-rtc
│   ├── test-keymap-util
│   ├── test-network
│   │   └── conf
│   │       ├── 10-dropin-test.netdev.d
│   │       ├── 11-test-unit-file.link.d
│   │       ├── 11-test-unit-file.netdev.d
│   │       ├── 11-test-unit-file.network.d
│   │       ├── 12-dummy.network.d
│   │       ├── 21-vlan-test1.network.d
│   │       ├── 21-vlan.netdev.d
│   │       ├── 25-activation-policy.network.d
│   │       ├── 25-address-ipv4acd-veth99.network.d
│   │       ├── 25-address-static.network.d
│   │       ├── 25-dhcp-client-allow-list.network.d
│   │       ├── 25-dhcp-client-ipv4-use-routes-use-gateway.network.d
│   │       ├── 25-neighbor-dummy.network.d
│   │       ├── 25-route-static-issue-35047.network.d
│   │       ├── 25-sysctl.network.d
│   │       ├── 25-test1.network.d
│   │       ├── 25-wireguard.netdev.d
│   │       ├── 26-bridge-vlan-master.network.d
│   │       ├── 26-bridge-vlan-slave.network.d
│   │       └── radvd
│   ├── test-network-generator-conversion
│   │   ├── test-01-dhcp.expected
│   │   ├── test-02-bridge.expected
│   │   └── test-03-issue-14319.expected
│   ├── test-path
│   ├── test-path-util
│   ├── test-resolve
│   ├── test-sysusers
│   ├── test-umount
│   ├── testdata -> .
│   └── units
│       ├── loopy.service.d
│       ├── TEST-55-OOMD-workload.slice.d
│       ├── unit-.service.d
│       ├── unit-with-.service.d
│       ├── unit-with-multiple-.service.d
│       └── unit-with-multiple-dashes.service.d
├── tmpfiles.d  : XXX - Defines directories, permissions, and ownerships created on boot (systemd-tmpfiles).
├── tools       : XXX - Utility scripts used in development, CI, or debugging. 
│   └── chromiumos
├── units   : XXX - All default systemd unit files (service, socket, timer, etc.) that ship with systemd.
│   ├── user
│   ├── user-.slice.d
│   ├── user@.service.d
│   └── user@0.service.d
└── xorg    : XXX - Configuration related to X.org integration — often minor or hardware-detection related.
