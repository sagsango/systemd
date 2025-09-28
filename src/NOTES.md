# XXX: These are all the services of the systemd :) enjoy!

/Users/sagarsingh/groot/kernel/systemd/src
├── ac-power
│   ├── ac-power.c
│   └── meson.build
├── analyze
│   ├── analyze-architectures.c
│   ├── analyze-architectures.h
│   ├── analyze-blame.c
│   ├── analyze-blame.h
│   ├── analyze-calendar.c
│   ├── analyze-calendar.h
│   ├── analyze-capability.c
│   ├── analyze-capability.h
│   ├── analyze-cat-config.c
│   ├── analyze-cat-config.h
│   ├── analyze-chid.c
│   ├── analyze-chid.h
│   ├── analyze-compare-versions.c
│   ├── analyze-compare-versions.h
│   ├── analyze-condition.c
│   ├── analyze-condition.h
│   ├── analyze-critical-chain.c
│   ├── analyze-critical-chain.h
│   ├── analyze-dot.c
│   ├── analyze-dot.h
│   ├── analyze-dump.c
│   ├── analyze-dump.h
│   ├── analyze-exit-status.c
│   ├── analyze-exit-status.h
│   ├── analyze-fdstore.c
│   ├── analyze-fdstore.h
│   ├── analyze-filesystems.c
│   ├── analyze-filesystems.h
│   ├── analyze-has-tpm2.c
│   ├── analyze-has-tpm2.h
│   ├── analyze-image-policy.c
│   ├── analyze-image-policy.h
│   ├── analyze-inspect-elf.c
│   ├── analyze-inspect-elf.h
│   ├── analyze-log-control.c
│   ├── analyze-log-control.h
│   ├── analyze-malloc.c
│   ├── analyze-malloc.h
│   ├── analyze-pcrs.c
│   ├── analyze-pcrs.h
│   ├── analyze-plot.c
│   ├── analyze-plot.h
│   ├── analyze-security.c
│   ├── analyze-security.h
│   ├── analyze-service-watchdogs.c
│   ├── analyze-service-watchdogs.h
│   ├── analyze-smbios11.c
│   ├── analyze-smbios11.h
│   ├── analyze-srk.c
│   ├── analyze-srk.h
│   ├── analyze-syscall-filter.c
│   ├── analyze-syscall-filter.h
│   ├── analyze-time-data.c
│   ├── analyze-time-data.h
│   ├── analyze-time.c
│   ├── analyze-time.h
│   ├── analyze-timespan.c
│   ├── analyze-timespan.h
│   ├── analyze-timestamp.c
│   ├── analyze-timestamp.h
│   ├── analyze-unit-files.c
│   ├── analyze-unit-files.h
│   ├── analyze-unit-paths.c
│   ├── analyze-unit-paths.h
│   ├── analyze-unit-shell.c
│   ├── analyze-unit-shell.h
│   ├── analyze-verify-util.c
│   ├── analyze-verify-util.h
│   ├── analyze-verify.c
│   ├── analyze-verify.h
│   ├── analyze.c
│   ├── analyze.h
│   ├── meson.build
│   └── test-verify.c
├── ask-password
│   ├── ask-password.c
│   ├── io.systemd.ask-password.policy
│   └── meson.build
├── backlight
│   ├── backlight.c
│   └── meson.build
├── basic
│   ├── af-list.c
│   ├── af-list.h
│   ├── af-to-name.awk
│   ├── alloc-util.c
│   ├── alloc-util.h
│   ├── ansi-color.c
│   ├── ansi-color.h
│   ├── architecture.c
│   ├── architecture.h
│   ├── argv-util.c
│   ├── argv-util.h
│   ├── arphrd-to-name.awk
│   ├── arphrd-util.c
│   ├── arphrd-util.h
│   ├── assert-util.c
│   ├── assert-util.h
│   ├── audit-util.c
│   ├── audit-util.h
│   ├── bitfield.h
│   ├── btrfs.c
│   ├── btrfs.h
│   ├── build-path.c
│   ├── build-path.h
│   ├── build.c
│   ├── build.h
│   ├── bus-label.c
│   ├── bus-label.h
│   ├── capability-list.c
│   ├── capability-list.h
│   ├── capability-to-name.awk
│   ├── capability-util.c
│   ├── capability-util.h
│   ├── capsule-util.c
│   ├── capsule-util.h
│   ├── cgroup-util.c
│   ├── cgroup-util.h
│   ├── chase.c
│   ├── chase.h
│   ├── chattr-util.c
│   ├── chattr-util.h
│   ├── check-filesystems.sh
│   ├── cleanup-util.h
│   ├── compress.c
│   ├── compress.h
│   ├── conf-files.c
│   ├── conf-files.h
│   ├── confidential-virt.c
│   ├── confidential-virt.h
│   ├── constants.h
│   ├── devnum-util.c
│   ├── devnum-util.h
│   ├── dirent-util.c
│   ├── dirent-util.h
│   ├── dlfcn-util.c
│   ├── dlfcn-util.h
│   ├── dns-def.h
│   ├── efivars.c
│   ├── efivars.h
│   ├── env-file.c
│   ├── env-file.h
│   ├── env-util.c
│   ├── env-util.h
│   ├── errno-list.c
│   ├── errno-list.h
│   ├── errno-to-name.awk
│   ├── errno-util.h
│   ├── escape.c
│   ├── escape.h
│   ├── ether-addr-util.c
│   ├── ether-addr-util.h
│   ├── extract-word.c
│   ├── extract-word.h
│   ├── fd-util.c
│   ├── fd-util.h
│   ├── fileio.c
│   ├── fileio.h
│   ├── filesystems-gperf.gperf
│   ├── filesystems.c
│   ├── filesystems.h
│   ├── format-ifname.c
│   ├── format-ifname.h
│   ├── format-util.c
│   ├── format-util.h
│   ├── forward.h
│   ├── fs-util.c
│   ├── fs-util.h
│   ├── gcrypt-util.c
│   ├── gcrypt-util.h
│   ├── generate-af-list.sh
│   ├── generate-arphrd-list.sh
│   ├── generate-capability-list.sh
│   ├── generate-errno-list.sh
│   ├── generate-filesystem-list.py
│   ├── generate-filesystem-switch-case.py
│   ├── getopt-defs.h
│   ├── glob-util.c
│   ├── glob-util.h
│   ├── glyph-util.c
│   ├── glyph-util.h
│   ├── gunicode.c
│   ├── gunicode.h
│   ├── hash-funcs.c
│   ├── hash-funcs.h
│   ├── hashmap.c
│   ├── hashmap.h
│   ├── hexdecoct.c
│   ├── hexdecoct.h
│   ├── hmac.c
│   ├── hmac.h
│   ├── hostname-util.c
│   ├── hostname-util.h
│   ├── in-addr-util.c
│   ├── in-addr-util.h
│   ├── initrd-util.c
│   ├── initrd-util.h
│   ├── inotify-util.c
│   ├── inotify-util.h
│   ├── io-util.c
│   ├── io-util.h
│   ├── iovec-util.c
│   ├── iovec-util.h
│   ├── iovec-wrapper.c
│   ├── iovec-wrapper.h
│   ├── iterator.h
│   ├── keyring-util.c
│   ├── keyring-util.h
│   ├── label.c
│   ├── label.h
│   ├── limits-util.c
│   ├── limits-util.h
│   ├── list.h
│   ├── locale-util.c
│   ├── locale-util.h
│   ├── lock-util.c
│   ├── lock-util.h
│   ├── log-context.c
│   ├── log-context.h
│   ├── log-ratelimit.h
│   ├── log.c
│   ├── log.h
│   ├── login-util.c
│   ├── login-util.h
│   ├── macro.h
│   ├── math-util.h
│   ├── memfd-util.c
│   ├── memfd-util.h
│   ├── memory-util.c
│   ├── memory-util.h
│   ├── mempool.c
│   ├── mempool.h
│   ├── memstream-util.c
│   ├── memstream-util.h
│   ├── meson.build
│   ├── missing-drm.h
│   ├── missing-network.h
│   ├── mkdir.c
│   ├── mkdir.h
│   ├── mountpoint-util.c
│   ├── mountpoint-util.h
│   ├── MurmurHash2.c
│   ├── MurmurHash2.h
│   ├── namespace-util.c
│   ├── namespace-util.h
│   ├── nss-util.h
│   ├── nulstr-util.c
│   ├── nulstr-util.h
│   ├── ordered-set.c
│   ├── ordered-set.h
│   ├── origin-id.h
│   ├── os-util.c
│   ├── os-util.h
│   ├── parse-util.c
│   ├── parse-util.h
│   ├── path-util.c
│   ├── path-util.h
│   ├── pcapng.h
│   ├── percent-util.c
│   ├── percent-util.h
│   ├── pidfd-util.c
│   ├── pidfd-util.h
│   ├── pidref.c
│   ├── pidref.h
│   ├── prioq.c
│   ├── prioq.h
│   ├── proc-cmdline.c
│   ├── proc-cmdline.h
│   ├── process-util.c
│   ├── process-util.h
│   ├── procfs-util.c
│   ├── procfs-util.h
│   ├── psi-util.c
│   ├── psi-util.h
│   ├── pthread-util.h
│   ├── random-util.c
│   ├── random-util.h
│   ├── ratelimit.c
│   ├── ratelimit.h
│   ├── raw-clone.c
│   ├── raw-clone.h
│   ├── recurse-dir.c
│   ├── recurse-dir.h
│   ├── replace-var.c
│   ├── replace-var.h
│   ├── rlimit-util.c
│   ├── rlimit-util.h
│   ├── runtime-scope.c
│   ├── runtime-scope.h
│   ├── set.h
│   ├── sha256.c
│   ├── sha256.h
│   ├── sigbus.c
│   ├── sigbus.h
│   ├── signal-util.c
│   ├── signal-util.h
│   ├── siphash24.c
│   ├── siphash24.h
│   ├── socket-util.c
│   ├── socket-util.h
│   ├── sort-util.c
│   ├── sort-util.h
│   ├── sparse-endian.h
│   ├── special.h
│   ├── stat-util.c
│   ├── stat-util.h
│   ├── static-destruct.c
│   ├── static-destruct.h
│   ├── stdio-util.h
│   ├── strbuf.c
│   ├── strbuf.h
│   ├── string-table.c
│   ├── string-table.h
│   ├── string-util.c
│   ├── string-util.h
│   ├── strv.c
│   ├── strv.h
│   ├── strxcpyx.c
│   ├── strxcpyx.h
│   ├── sync-util.c
│   ├── sync-util.h
│   ├── sysctl-util.c
│   ├── sysctl-util.h
│   ├── syslog-util.c
│   ├── syslog-util.h
│   ├── terminal-util.c
│   ├── terminal-util.h
│   ├── time-util.c
│   ├── time-util.h
│   ├── tmpfile-util.c
│   ├── tmpfile-util.h
│   ├── uid-classification.c
│   ├── uid-classification.h
│   ├── uid-range.c
│   ├── uid-range.h
│   ├── umask-util.h
│   ├── unaligned.h
│   ├── unit-def.c
│   ├── unit-def.h
│   ├── unit-name.c
│   ├── unit-name.h
│   ├── user-util.c
│   ├── user-util.h
│   ├── utf8.c
│   ├── utf8.h
│   ├── virt.c
│   ├── virt.h
│   ├── xattr-util.c
│   └── xattr-util.h
├── battery-check
│   ├── battery-check.c
│   └── meson.build
├── binfmt
│   ├── binfmt.c
│   └── meson.build
├── bless-boot
│   ├── bless-boot-generator.c
│   ├── bless-boot.c
│   ├── boot-check-no-failures.c
│   └── meson.build
├── boot
│   ├── addon.c
│   ├── bcd.c
│   ├── bcd.h
│   ├── boot.c
│   ├── chid.c
│   ├── chid.h
│   ├── console.c
│   ├── console.h
│   ├── cpio.c
│   ├── cpio.h
│   ├── device-path-util.c
│   ├── device-path-util.h
│   ├── devicetree.c
│   ├── devicetree.h
│   ├── drivers.c
│   ├── drivers.h
│   ├── edid.c
│   ├── edid.h
│   ├── efi-efivars.c
│   ├── efi-efivars.h
│   ├── efi-firmware.c
│   ├── efi-firmware.h
│   ├── efi-log.c
│   ├── efi-log.h
│   ├── efi-string-table.h
│   ├── efi-string.c
│   ├── efi-string.h
│   ├── efi.h
│   ├── export-vars.c
│   ├── export-vars.h
│   ├── fuzz-bcd.c
│   ├── fuzz-efi-osrel.c
│   ├── fuzz-efi-printf.c
│   ├── fuzz-efi-string.c
│   ├── generate-hwids-section.py
│   ├── graphics.c
│   ├── graphics.h
│   ├── hwids
│   │   ├── device1.json
│   │   ├── device2.json
│   │   ├── device3.json
│   │   └── device4.json
│   ├── initrd.c
│   ├── initrd.h
│   ├── line-edit.c
│   ├── line-edit.h
│   ├── linux_x86.c
│   ├── linux.c
│   ├── linux.h
│   ├── measure.c
│   ├── measure.h
│   ├── meson.build
│   ├── part-discovery.c
│   ├── part-discovery.h
│   ├── pe.c
│   ├── pe.h
│   ├── proto
│   │   ├── block-io.h
│   │   ├── cc-measurement.h
│   │   ├── console-control.h
│   │   ├── device-path.h
│   │   ├── dt-fixup.h
│   │   ├── edid-discovered.h
│   │   ├── file-io.h
│   │   ├── graphics-output.h
│   │   ├── load-file.h
│   │   ├── loaded-image.h
│   │   ├── rng.h
│   │   ├── security-arch.h
│   │   ├── shell-parameters.h
│   │   ├── simple-text-io.h
│   │   └── tcg.h
│   ├── random-seed.c
│   ├── random-seed.h
│   ├── secure-boot.c
│   ├── secure-boot.h
│   ├── shim.c
│   ├── shim.h
│   ├── smbios.c
│   ├── smbios.h
│   ├── splash.c
│   ├── splash.h
│   ├── stub.c
│   ├── sysfail.c
│   ├── sysfail.h
│   ├── test-bcd.c
│   ├── test-chid-match.c
│   ├── test-efi-string.c
│   ├── ticks.c
│   ├── ticks.h
│   ├── ubsan.c
│   ├── UEFI_SECURITY.md
│   ├── url-discovery.c
│   ├── url-discovery.h
│   ├── util.c
│   ├── util.h
│   ├── vmm.c
│   └── vmm.h
├── bootctl
│   ├── bootctl-install.c
│   ├── bootctl-install.h
│   ├── bootctl-random-seed.c
│   ├── bootctl-random-seed.h
│   ├── bootctl-reboot-to-firmware.c
│   ├── bootctl-reboot-to-firmware.h
│   ├── bootctl-set-efivar.c
│   ├── bootctl-set-efivar.h
│   ├── bootctl-status.c
│   ├── bootctl-status.h
│   ├── bootctl-uki.c
│   ├── bootctl-uki.h
│   ├── bootctl-util.c
│   ├── bootctl-util.h
│   ├── bootctl.c
│   ├── bootctl.h
│   └── meson.build
├── busctl
│   ├── busctl-introspect.c
│   ├── busctl-introspect.h
│   ├── busctl.c
│   ├── meson.build
│   └── test-busctl-introspect.c
├── cgls
│   ├── cgls.c
│   └── meson.build
├── cgtop
│   ├── cgtop.c
│   └── meson.build
├── core
│   ├── all-units.h
│   ├── apparmor-setup.c
│   ├── apparmor-setup.h
│   ├── audit-fd.c
│   ├── audit-fd.h
│   ├── automount.c
│   ├── automount.h
│   ├── bpf
│   │   ├── restrict-fs
│   │   │   ├── meson.build
│   │   │   ├── restrict-fs-skel.h
│   │   │   └── restrict-fs.bpf.c
│   │   ├── restrict-ifaces
│   │   │   ├── meson.build
│   │   │   ├── restrict-ifaces-skel.h
│   │   │   └── restrict-ifaces.bpf.c
│   │   └── socket-bind
│   │       ├── meson.build
│   │       ├── socket-bind-api.bpf.h
│   │       ├── socket-bind-skel.h
│   │       └── socket-bind.bpf.c
│   ├── bpf-devices.c
│   ├── bpf-devices.h
│   ├── bpf-firewall.c
│   ├── bpf-firewall.h
│   ├── bpf-foreign.c
│   ├── bpf-foreign.h
│   ├── bpf-restrict-fs.c
│   ├── bpf-restrict-fs.h
│   ├── bpf-restrict-ifaces.c
│   ├── bpf-restrict-ifaces.h
│   ├── bpf-socket-bind.c
│   ├── bpf-socket-bind.h
│   ├── cgroup.c
│   ├── cgroup.h
│   ├── clock-warp.c
│   ├── clock-warp.h
│   ├── core-forward.h
│   ├── crash-handler.c
│   ├── crash-handler.h
│   ├── dbus-automount.c
│   ├── dbus-automount.h
│   ├── dbus-cgroup.c
│   ├── dbus-cgroup.h
│   ├── dbus-device.c
│   ├── dbus-device.h
│   ├── dbus-execute.c
│   ├── dbus-execute.h
│   ├── dbus-job.c
│   ├── dbus-job.h
│   ├── dbus-kill.c
│   ├── dbus-kill.h
│   ├── dbus-manager.c
│   ├── dbus-manager.h
│   ├── dbus-mount.c
│   ├── dbus-mount.h
│   ├── dbus-path.c
│   ├── dbus-path.h
│   ├── dbus-scope.c
│   ├── dbus-scope.h
│   ├── dbus-service.c
│   ├── dbus-service.h
│   ├── dbus-slice.c
│   ├── dbus-slice.h
│   ├── dbus-socket.c
│   ├── dbus-socket.h
│   ├── dbus-swap.c
│   ├── dbus-swap.h
│   ├── dbus-target.c
│   ├── dbus-target.h
│   ├── dbus-timer.c
│   ├── dbus-timer.h
│   ├── dbus-unit.c
│   ├── dbus-unit.h
│   ├── dbus-util.c
│   ├── dbus-util.h
│   ├── dbus.c
│   ├── dbus.h
│   ├── device.c
│   ├── device.h
│   ├── dynamic-user.c
│   ├── dynamic-user.h
│   ├── efi-random.c
│   ├── efi-random.h
│   ├── emergency-action.c
│   ├── emergency-action.h
│   ├── exec-credential.c
│   ├── exec-credential.h
│   ├── exec-invoke.c
│   ├── exec-invoke.h
│   ├── execute-serialize.c
│   ├── execute-serialize.h
│   ├── execute.c
│   ├── execute.h
│   ├── executor.c
│   ├── fuzz-execute-serialize.c
│   ├── fuzz-manager-serialize.c
│   ├── fuzz-manager-serialize.options
│   ├── fuzz-unit-file.c
│   ├── fuzz-unit-file.options
│   ├── generate-bpf-delegate-configs.py
│   ├── generator-setup.c
│   ├── generator-setup.h
│   ├── ima-setup.c
│   ├── ima-setup.h
│   ├── import-creds.c
│   ├── import-creds.h
│   ├── ipe-setup.c
│   ├── ipe-setup.h
│   ├── job.c
│   ├── job.h
│   ├── kill.c
│   ├── kill.h
│   ├── kmod-setup.c
│   ├── kmod-setup.h
│   ├── load-dropin.c
│   ├── load-dropin.h
│   ├── load-fragment-gperf-nulstr.awk
│   ├── load-fragment-gperf.gperf.in
│   ├── load-fragment.c
│   ├── load-fragment.h
│   ├── main.c
│   ├── main.h
│   ├── manager-dump.c
│   ├── manager-dump.h
│   ├── manager-serialize.c
│   ├── manager-serialize.h
│   ├── manager.c
│   ├── manager.h
│   ├── meson.build
│   ├── mount.c
│   ├── mount.h
│   ├── namespace.c
│   ├── namespace.h
│   ├── org.freedesktop.systemd1.conf
│   ├── org.freedesktop.systemd1.policy.in
│   ├── org.freedesktop.systemd1.service
│   ├── path.c
│   ├── path.h
│   ├── scope.c
│   ├── scope.h
│   ├── selinux-access.c
│   ├── selinux-access.h
│   ├── selinux-setup.c
│   ├── selinux-setup.h
│   ├── service.c
│   ├── service.h
│   ├── show-status.c
│   ├── show-status.h
│   ├── slice.c
│   ├── slice.h
│   ├── smack-setup.c
│   ├── smack-setup.h
│   ├── socket.c
│   ├── socket.h
│   ├── swap.c
│   ├── swap.h
│   ├── system.conf.in
│   ├── systemd.pc.in
│   ├── taint.c
│   ├── taint.h
│   ├── target.c
│   ├── target.h
│   ├── timer.c
│   ├── timer.h
│   ├── transaction.c
│   ├── transaction.h
│   ├── unit-dependency-atom.c
│   ├── unit-dependency-atom.h
│   ├── unit-printf.c
│   ├── unit-printf.h
│   ├── unit-serialize.c
│   ├── unit-serialize.h
│   ├── unit.c
│   ├── unit.h
│   ├── user.conf.in
│   ├── varlink-cgroup.c
│   ├── varlink-cgroup.h
│   ├── varlink-common.c
│   ├── varlink-common.h
│   ├── varlink-dynamic-user.c
│   ├── varlink-dynamic-user.h
│   ├── varlink-manager.c
│   ├── varlink-manager.h
│   ├── varlink-unit.c
│   ├── varlink-unit.h
│   ├── varlink.c
│   └── varlink.h
├── coredump
│   ├── coredump-vacuum.c
│   ├── coredump-vacuum.h
│   ├── coredump.c
│   ├── coredump.conf
│   ├── coredumpctl.c
│   ├── meson.build
│   └── test-coredump-vacuum.c
├── coverage
│   ├── coverage.h
│   └── meson.build
├── creds
│   ├── creds.c
│   ├── io.systemd.credentials.policy
│   └── meson.build
├── cryptenroll
│   ├── cryptenroll-fido2.c
│   ├── cryptenroll-fido2.h
│   ├── cryptenroll-list.c
│   ├── cryptenroll-list.h
│   ├── cryptenroll-password.c
│   ├── cryptenroll-password.h
│   ├── cryptenroll-pkcs11.c
│   ├── cryptenroll-pkcs11.h
│   ├── cryptenroll-recovery.c
│   ├── cryptenroll-recovery.h
│   ├── cryptenroll-tpm2.c
│   ├── cryptenroll-tpm2.h
│   ├── cryptenroll-wipe.c
│   ├── cryptenroll-wipe.h
│   ├── cryptenroll.c
│   ├── cryptenroll.h
│   └── meson.build
├── cryptsetup
│   ├── cryptsetup-generator.c
│   ├── cryptsetup-keyfile.c
│   ├── cryptsetup-keyfile.h
│   ├── cryptsetup-pkcs11.c
│   ├── cryptsetup-pkcs11.h
│   ├── cryptsetup-tokens
│   │   ├── cryptsetup-token-systemd-fido2.c
│   │   ├── cryptsetup-token-systemd-pkcs11.c
│   │   ├── cryptsetup-token-systemd-tpm2.c
│   │   ├── cryptsetup-token-util.c
│   │   ├── cryptsetup-token-util.h
│   │   ├── cryptsetup-token.h
│   │   ├── cryptsetup-token.sym
│   │   ├── luks2-fido2.c
│   │   ├── luks2-fido2.h
│   │   ├── luks2-pkcs11.c
│   │   ├── luks2-pkcs11.h
│   │   ├── luks2-tpm2.c
│   │   ├── luks2-tpm2.h
│   │   └── meson.build
│   ├── cryptsetup.c
│   └── meson.build
├── debug-generator
│   ├── debug-generator.c
│   └── meson.build
├── delta
│   ├── delta.c
│   └── meson.build
├── detect-virt
│   ├── detect-virt.c
│   └── meson.build
├── dissect
│   ├── dissect.c
│   └── meson.build
├── environment-d-generator
│   ├── environment-d-generator.c
│   └── meson.build
├── escape
│   ├── escape-tool.c
│   └── meson.build
├── factory-reset
│   ├── factory-reset-generator.c
│   ├── factory-reset-tool.c
│   └── meson.build
├── firstboot               XXX: TODO
│   ├── firstboot.c
│   └── meson.build
├── fsck
│   ├── fsck.c
│   └── meson.build
├── fstab-generator
│   ├── fstab-generator.c
│   └── meson.build
├── fundamental
│   ├── assert-fundamental.h
│   ├── bootspec-fundamental.c
│   ├── bootspec-fundamental.h
│   ├── chid-fundamental.c
│   ├── chid-fundamental.h
│   ├── cleanup-fundamental.h
│   ├── confidential-virt-fundamental.h
│   ├── edid-fundamental.c
│   ├── edid-fundamental.h
│   ├── efi-fundamental.h
│   ├── efivars-fundamental.c
│   ├── efivars-fundamental.h
│   ├── iovec-util-fundamental.h
│   ├── logarithm.h
│   ├── macro-fundamental.h
│   ├── memory-util-fundamental.h
│   ├── meson.build
│   ├── sbat.h
│   ├── sha1-fundamental.c
│   ├── sha1-fundamental.h
│   ├── sha256-fundamental.c
│   ├── sha256-fundamental.h
│   ├── string-util-fundamental.c
│   ├── string-util-fundamental.h
│   ├── strv-fundamental.h
│   ├── tpm2-pcr.h
│   ├── uki.c
│   ├── uki.h
│   └── unaligned-fundamental.h
├── fuzz
│   ├── fuzz-bootspec-gen.py
│   ├── fuzz-bootspec.c
│   ├── fuzz-bootspec.options
│   ├── fuzz-bus-label.c
│   ├── fuzz-calendarspec.c
│   ├── fuzz-catalog.c
│   ├── fuzz-compress.c
│   ├── fuzz-env-file.c
│   ├── fuzz-env-file.options
│   ├── fuzz-hostname-setup.c
│   ├── fuzz-json.c
│   ├── fuzz-main.c
│   ├── fuzz-time-util.c
│   ├── fuzz-udev-database.c
│   ├── fuzz-varlink-idl.c
│   ├── fuzz-varlink.c
│   ├── fuzz.h
│   └── meson.build
├── getty-generator
│   ├── getty-generator.c
│   └── meson.build
├── gpt-auto-generator
│   ├── gpt-auto-generator.c
│   └── meson.build
├── growfs
│   ├── growfs.c
│   ├── makefs.c
│   └── meson.build
├── hibernate-resume
│   ├── hibernate-resume-config.c
│   ├── hibernate-resume-config.h
│   ├── hibernate-resume-generator.c
│   ├── hibernate-resume.c
│   └── meson.build
├── home
│   ├── home-util.c
│   ├── home-util.h
│   ├── homectl-fido2.c
│   ├── homectl-fido2.h
│   ├── homectl-pkcs11.c
│   ├── homectl-pkcs11.h
│   ├── homectl-recovery-key.c
│   ├── homectl-recovery-key.h
│   ├── homectl.c
│   ├── homed-bus.c
│   ├── homed-bus.h
│   ├── homed-conf.c
│   ├── homed-conf.h
│   ├── homed-forward.h
│   ├── homed-gperf.gperf
│   ├── homed-home-bus.c
│   ├── homed-home-bus.h
│   ├── homed-home.c
│   ├── homed-home.h
│   ├── homed-manager-bus.c
│   ├── homed-manager-bus.h
│   ├── homed-manager.c
│   ├── homed-manager.h
│   ├── homed-operation.c
│   ├── homed-operation.h
│   ├── homed-varlink.c
│   ├── homed-varlink.h
│   ├── homed.c
│   ├── homed.conf
│   ├── homework-blob.c
│   ├── homework-blob.h
│   ├── homework-cifs.c
│   ├── homework-cifs.h
│   ├── homework-directory.c
│   ├── homework-directory.h
│   ├── homework-fido2.c
│   ├── homework-fido2.h
│   ├── homework-forward.h
│   ├── homework-fscrypt.c
│   ├── homework-fscrypt.h
│   ├── homework-luks.c
│   ├── homework-luks.h
│   ├── homework-mount.c
│   ├── homework-mount.h
│   ├── homework-password-cache.c
│   ├── homework-password-cache.h
│   ├── homework-pkcs11.c
│   ├── homework-pkcs11.h
│   ├── homework-quota.c
│   ├── homework-quota.h
│   ├── homework.c
│   ├── homework.h
│   ├── meson.build
│   ├── org.freedesktop.home1.conf
│   ├── org.freedesktop.home1.policy
│   ├── org.freedesktop.home1.service
│   ├── pam_systemd_home.c
│   ├── pam_systemd_home.sym
│   ├── test-homed-regression-31896.c
│   ├── user-record-password-quality.c
│   ├── user-record-password-quality.h
│   ├── user-record-sign.c
│   ├── user-record-sign.h
│   ├── user-record-util.c
│   └── user-record-util.h
├── hostname
│   ├── hostnamectl.c
│   ├── hostnamed.c
│   ├── meson.build
│   ├── org.freedesktop.hostname1.conf
│   ├── org.freedesktop.hostname1.policy
│   └── org.freedesktop.hostname1.service
├── hwdb
│   ├── hwdb.c
│   └── meson.build
├── id128
│   ├── id128.c
│   └── meson.build
├── import
│   ├── curl-util.c
│   ├── curl-util.h
│   ├── export-raw.c
│   ├── export-raw.h
│   ├── export-tar.c
│   ├── export-tar.h
│   ├── export.c
│   ├── import-common.c
│   ├── import-common.h
│   ├── import-compress.c
│   ├── import-compress.h
│   ├── import-fs.c
│   ├── import-generator.c
│   ├── import-pubring.pgp
│   ├── import-raw.c
│   ├── import-raw.h
│   ├── import-tar.c
│   ├── import-tar.h
│   ├── import.c
│   ├── importctl.c
│   ├── importd.c
│   ├── meson.build
│   ├── org.freedesktop.import1.conf
│   ├── org.freedesktop.import1.policy
│   ├── org.freedesktop.import1.service
│   ├── pull-common.c
│   ├── pull-common.h
│   ├── pull-job.c
│   ├── pull-job.h
│   ├── pull-raw.c
│   ├── pull-raw.h
│   ├── pull-tar.c
│   ├── pull-tar.h
│   ├── pull.c
│   ├── qcow2-util.c
│   ├── qcow2-util.h
│   └── test-qcow2.c
├── include
│   ├── meson.build
│   ├── override
│   │   ├── fcntl.h
│   │   ├── linux
│   │   │   ├── audit.h
│   │   │   ├── bpf.h
│   │   │   ├── fs.h
│   │   │   ├── keyctl.h
│   │   │   ├── magic.h
│   │   │   ├── nsfs.h
│   │   │   └── xfs.h
│   │   ├── malloc.h
│   │   ├── net
│   │   │   ├── if_arp.h
│   │   │   └── if.h
│   │   ├── netinet
│   │   │   └── in.h
│   │   ├── sched.h
│   │   ├── signal.h
│   │   ├── sys
│   │   │   ├── bpf.h
│   │   │   ├── generate-syscall.py
│   │   │   ├── ioprio.h
│   │   │   ├── kcmp.h
│   │   │   ├── keyctl.h
│   │   │   ├── mempolicy.h
│   │   │   ├── meson.build
│   │   │   ├── mman.h
│   │   │   ├── mount.h
│   │   │   ├── param.h
│   │   │   ├── pidfd.h
│   │   │   ├── quota.h
│   │   │   ├── random.h
│   │   │   ├── socket.h
│   │   │   ├── stat.h
│   │   │   ├── syscall-list.txt
│   │   │   ├── syscall.h
│   │   │   ├── syscalls-alpha.txt
│   │   │   ├── syscalls-arc.txt
│   │   │   ├── syscalls-arm.txt
│   │   │   ├── syscalls-arm64.txt
│   │   │   ├── syscalls-i386.txt
│   │   │   ├── syscalls-ia64.txt
│   │   │   ├── syscalls-loongarch64.txt
│   │   │   ├── syscalls-m68k.txt
│   │   │   ├── syscalls-mips64.txt
│   │   │   ├── syscalls-mips64n32.txt
│   │   │   ├── syscalls-mipso32.txt
│   │   │   ├── syscalls-parisc.txt
│   │   │   ├── syscalls-powerpc.txt
│   │   │   ├── syscalls-powerpc64.txt
│   │   │   ├── syscalls-riscv32.txt
│   │   │   ├── syscalls-riscv64.txt
│   │   │   ├── syscalls-s390.txt
│   │   │   ├── syscalls-s390x.txt
│   │   │   ├── syscalls-sparc.txt
│   │   │   ├── syscalls-x86_64.txt
│   │   │   ├── wait.h
│   │   │   └── xattr.h
│   │   └── unistd.h
│   └── uapi
│       └── linux
│           ├── auto_dev-ioctl.h
│           ├── auto_fs.h
│           ├── batman_adv.h
│           ├── bpf_common.h
│           ├── bpf_insn.h
│           ├── bpf.h
│           ├── btrfs_tree.h
│           ├── btrfs.h
│           ├── can
│           │   ├── netlink.h
│           │   └── vxcan.h
│           ├── capability.h
│           ├── cfm_bridge.h
│           ├── const.h
│           ├── dm-ioctl.h
│           ├── ethtool.h
│           ├── fib_rules.h
│           ├── filter.h
│           ├── fou.h
│           ├── fs.h
│           ├── fscrypt.h
│           ├── fsverity.h
│           ├── genetlink.h
│           ├── hdlc
│           │   └── ioctl.h
│           ├── hid.h
│           ├── hidraw.h
│           ├── if_addr.h
│           ├── if_addrlabel.h
│           ├── if_arp.h
│           ├── if_bonding.h
│           ├── if_bridge.h
│           ├── if_ether.h
│           ├── if_infiniband.h
│           ├── if_link.h
│           ├── if_macsec.h
│           ├── if_packet.h
│           ├── if_tun.h
│           ├── if_tunnel.h
│           ├── if_vlan.h
│           ├── if.h
│           ├── in.h
│           ├── in6.h
│           ├── input-event-codes.h
│           ├── input.h
│           ├── ioprio.h
│           ├── ip.h
│           ├── ip6_tunnel.h
│           ├── ipv6_route.h
│           ├── ipv6.h
│           ├── keyctl.h
│           ├── l2tp.h
│           ├── libc-compat.h
│           ├── limits.h
│           ├── loop.h
│           ├── magic.h
│           ├── mempolicy.h
│           ├── mount.h
│           ├── mrp_bridge.h
│           ├── neighbour.h
│           ├── net_namespace.h
│           ├── netdevice.h
│           ├── netfilter
│           │   ├── nf_conntrack_common.h
│           │   ├── nf_conntrack_tuple_common.h
│           │   ├── nf_nat.h
│           │   ├── nf_tables.h
│           │   ├── nfnetlink_compat.h
│           │   ├── nfnetlink.h
│           │   ├── x_tables.h
│           │   ├── xt_addrtype.h
│           │   └── xt_tcpudp.h
│           ├── netfilter_ipv4
│           │   └── ip_tables.h
│           ├── netfilter_ipv4.h
│           ├── netfilter.h
│           ├── netlink.h
│           ├── nexthop.h
│           ├── nl80211.h
│           ├── pkt_sched.h
│           ├── prctl.h
│           ├── rtnetlink.h
│           ├── sched
│           │   └── types.h
│           ├── socket.h
│           ├── sockios.h
│           ├── stat.h
│           ├── stddef.h
│           ├── update.sh
│           ├── veth.h
│           ├── vm_sockets.h
│           ├── wireguard.h
│           └── xattr.h
├── integritysetup
│   ├── integrity-util.c
│   ├── integrity-util.h
│   ├── integritysetup-generator.c
│   ├── integritysetup.c
│   └── meson.build
├── journal
│   ├── bsod.c
│   ├── cat.c
│   ├── fuzz-journald-audit.c
│   ├── fuzz-journald-kmsg.c
│   ├── fuzz-journald-native-fd.c
│   ├── fuzz-journald-native.c
│   ├── fuzz-journald-stream.c
│   ├── fuzz-journald-stream.options
│   ├── fuzz-journald-syslog.c
│   ├── fuzz-journald.c
│   ├── fuzz-journald.h
│   ├── journalctl-authenticate.c
│   ├── journalctl-authenticate.h
│   ├── journalctl-catalog.c
│   ├── journalctl-catalog.h
│   ├── journalctl-filter.c
│   ├── journalctl-filter.h
│   ├── journalctl-misc.c
│   ├── journalctl-misc.h
│   ├── journalctl-show.c
│   ├── journalctl-show.h
│   ├── journalctl-util.c
│   ├── journalctl-util.h
│   ├── journalctl-varlink.c
│   ├── journalctl-varlink.h
│   ├── journalctl.c
│   ├── journalctl.h
│   ├── journald-audit.c
│   ├── journald-audit.h
│   ├── journald-client.c
│   ├── journald-client.h
│   ├── journald-console.c
│   ├── journald-console.h
│   ├── journald-context.c
│   ├── journald-context.h
│   ├── journald-forward.h
│   ├── journald-gperf.gperf
│   ├── journald-kmsg.c
│   ├── journald-kmsg.h
│   ├── journald-manager.c
│   ├── journald-manager.h
│   ├── journald-native.c
│   ├── journald-native.h
│   ├── journald-rate-limit.c
│   ├── journald-rate-limit.h
│   ├── journald-socket.c
│   ├── journald-socket.h
│   ├── journald-stream.c
│   ├── journald-stream.h
│   ├── journald-sync.c
│   ├── journald-sync.h
│   ├── journald-syslog.c
│   ├── journald-syslog.h
│   ├── journald-varlink.c
│   ├── journald-varlink.h
│   ├── journald-wall.c
│   ├── journald-wall.h
│   ├── journald.c
│   ├── journald.conf
│   ├── meson.build
│   ├── test-journald-config.c
│   ├── test-journald-rate-limit.c
│   ├── test-journald-syslog.c
│   └── test-journald-tables.c
├── journal-remote
│   ├── browse.html
│   ├── fuzz-journal-remote.c
│   ├── fuzz-journal-remote.options
│   ├── journal-compression-util.c
│   ├── journal-compression-util.h
│   ├── journal-gatewayd.c
│   ├── journal-header-util.c
│   ├── journal-header-util.h
│   ├── journal-remote-main.c
│   ├── journal-remote-parse.c
│   ├── journal-remote-parse.h
│   ├── journal-remote-write.c
│   ├── journal-remote-write.h
│   ├── journal-remote.c
│   ├── journal-remote.conf.in
│   ├── journal-remote.h
│   ├── journal-upload-journal.c
│   ├── journal-upload.c
│   ├── journal-upload.conf.in
│   ├── journal-upload.h
│   ├── log-generator.py
│   ├── meson.build
│   ├── microhttpd-util.c
│   ├── microhttpd-util.h
│   └── test-journal-header-util.c
├── kernel-install
│   ├── 50-depmod.install
│   ├── 60-ukify.install.in
│   ├── 90-loaderentry.install.in
│   ├── 90-uki-copy.install
│   ├── install.conf
│   ├── kernel-install.c
│   ├── meson.build
│   ├── test-kernel-install.sh
│   └── uki.conf
├── keyutil
│   ├── keyutil.c
│   └── meson.build
├── libc
│   ├── bpf.c
│   ├── ioprio.c
│   ├── kcmp.c
│   ├── keyctl.c
│   ├── mempolicy.c
│   ├── meson.build
│   ├── mount.c
│   ├── pidfd.c
│   ├── quota.c
│   ├── sched.c
│   ├── signal.c
│   ├── stat.c
│   ├── unistd.c
│   └── xattr.c
├── libsystemd
│   ├── libsystemd.pc.in
│   ├── libsystemd.sym
│   ├── meson.build
│   ├── sd-bus
│   │   ├── bus-common-errors.c
│   │   ├── bus-common-errors.h
│   │   ├── bus-container.c
│   │   ├── bus-container.h
│   │   ├── bus-control.c
│   │   ├── bus-control.h
│   │   ├── bus-convenience.c
│   │   ├── bus-creds.c
│   │   ├── bus-creds.h
│   │   ├── bus-dump-json.c
│   │   ├── bus-dump.c
│   │   ├── bus-dump.h
│   │   ├── bus-error.c
│   │   ├── bus-error.h
│   │   ├── bus-forward.h
│   │   ├── bus-internal.c
│   │   ├── bus-internal.h
│   │   ├── bus-introspect.c
│   │   ├── bus-introspect.h
│   │   ├── bus-kernel.c
│   │   ├── bus-kernel.h
│   │   ├── bus-match.c
│   │   ├── bus-match.h
│   │   ├── bus-message.c
│   │   ├── bus-message.h
│   │   ├── bus-objects.c
│   │   ├── bus-objects.h
│   │   ├── bus-protocol.h
│   │   ├── bus-signature.c
│   │   ├── bus-signature.h
│   │   ├── bus-slot.c
│   │   ├── bus-slot.h
│   │   ├── bus-socket.c
│   │   ├── bus-socket.h
│   │   ├── bus-track.c
│   │   ├── bus-track.h
│   │   ├── bus-type.c
│   │   ├── bus-type.h
│   │   ├── fuzz-bus-match.c
│   │   ├── fuzz-bus-match.options
│   │   ├── fuzz-bus-message.c
│   │   ├── sd-bus.c
│   │   ├── test-bus-address.c
│   │   ├── test-bus-benchmark.c
│   │   ├── test-bus-chat.c
│   │   ├── test-bus-cleanup.c
│   │   ├── test-bus-creds.c
│   │   ├── test-bus-error.c
│   │   ├── test-bus-introspect.c
│   │   ├── test-bus-marshal.c
│   │   ├── test-bus-match.c
│   │   ├── test-bus-objects.c
│   │   ├── test-bus-peersockaddr.c
│   │   ├── test-bus-queue-ref-cycle.c
│   │   ├── test-bus-server.c
│   │   ├── test-bus-signature.c
│   │   ├── test-bus-track.c
│   │   ├── test-bus-vtable-cc.cc -> test-bus-vtable.c
│   │   ├── test-bus-vtable.c
│   │   ├── test-bus-watch-bind.c
│   │   └── test-vtable-data.h
│   ├── sd-daemon
│   │   └── sd-daemon.c
│   ├── sd-device
│   │   ├── device-enumerator-private.h
│   │   ├── device-enumerator.c
│   │   ├── device-filter.c
│   │   ├── device-filter.h
│   │   ├── device-internal.h
│   │   ├── device-monitor-private.h
│   │   ├── device-monitor.c
│   │   ├── device-private.c
│   │   ├── device-private.h
│   │   ├── device-util.c
│   │   ├── device-util.h
│   │   ├── sd-device.c
│   │   ├── test-device-util.c
│   │   ├── test-sd-device-monitor.c
│   │   ├── test-sd-device-thread.c
│   │   └── test-sd-device.c
│   ├── sd-event
│   │   ├── event-source.h
│   │   ├── event-util.c
│   │   ├── event-util.h
│   │   ├── sd-event.c
│   │   └── test-event.c
│   ├── sd-hwdb
│   │   ├── hwdb-internal.h
│   │   └── sd-hwdb.c
│   ├── sd-id128
│   │   ├── id128-util.c
│   │   ├── id128-util.h
│   │   └── sd-id128.c
│   ├── sd-journal
│   │   ├── audit_type-to-name.awk
│   │   ├── audit-type.c
│   │   ├── audit-type.h
│   │   ├── catalog.c
│   │   ├── catalog.h
│   │   ├── fsprg.c
│   │   ├── fsprg.h
│   │   ├── generate-audit_type-list.sh
│   │   ├── journal-authenticate.c
│   │   ├── journal-authenticate.h
│   │   ├── journal-def.h
│   │   ├── journal-file.c
│   │   ├── journal-file.h
│   │   ├── journal-internal.h
│   │   ├── journal-send.c
│   │   ├── journal-send.h
│   │   ├── journal-vacuum.c
│   │   ├── journal-vacuum.h
│   │   ├── journal-verify.c
│   │   ├── journal-verify.h
│   │   ├── lookup3.c
│   │   ├── lookup3.h
│   │   ├── meson.build
│   │   ├── mmap-cache.c
│   │   ├── mmap-cache.h
│   │   ├── sd-journal.c
│   │   ├── test-audit-type.c
│   │   ├── test-catalog.c
│   │   ├── test-journal-append.c
│   │   ├── test-journal-enum.c
│   │   ├── test-journal-file.c
│   │   ├── test-journal-flush.c
│   │   ├── test-journal-init.c
│   │   ├── test-journal-interleaving.c
│   │   ├── test-journal-match.c
│   │   ├── test-journal-send.c
│   │   ├── test-journal-stream.c
│   │   ├── test-journal-verify.c
│   │   ├── test-journal.c
│   │   └── test-mmap-cache.c
│   ├── sd-json
│   │   ├── json-internal.h
│   │   ├── json-util.c
│   │   ├── json-util.h
│   │   └── sd-json.c
│   ├── sd-login
│   │   ├── sd-login.c
│   │   ├── test-login.c
│   │   └── test-sd-login.c
│   ├── sd-netlink
│   │   ├── netlink-genl.c
│   │   ├── netlink-genl.h
│   │   ├── netlink-internal.h
│   │   ├── netlink-message-nfnl.c
│   │   ├── netlink-message-rtnl.c
│   │   ├── netlink-message.c
│   │   ├── netlink-slot.c
│   │   ├── netlink-slot.h
│   │   ├── netlink-sock-diag.c
│   │   ├── netlink-sock-diag.h
│   │   ├── netlink-socket.c
│   │   ├── netlink-types-genl.c
│   │   ├── netlink-types-internal.h
│   │   ├── netlink-types-nfnl.c
│   │   ├── netlink-types-rtnl.c
│   │   ├── netlink-types-sdnl.c
│   │   ├── netlink-types.c
│   │   ├── netlink-types.h
│   │   ├── netlink-util.c
│   │   ├── netlink-util.h
│   │   ├── sd-netlink.c
│   │   └── test-netlink.c
│   ├── sd-network
│   │   ├── network-util.c
│   │   ├── network-util.h
│   │   └── sd-network.c
│   ├── sd-path
│   │   ├── path-lookup.c
│   │   ├── path-lookup.h
│   │   └── sd-path.c
│   ├── sd-resolve
│   │   ├── resolve-private.h
│   │   ├── sd-resolve.c
│   │   └── test-resolve.c
│   └── sd-varlink
│       ├── sd-varlink-idl.c
│       ├── sd-varlink.c
│       ├── varlink-idl-util.h
│       ├── varlink-internal.h
│       ├── varlink-io.systemd.c
│       ├── varlink-io.systemd.h
│       ├── varlink-org.varlink.service.c
│       ├── varlink-org.varlink.service.h
│       ├── varlink-util.c
│       └── varlink-util.h
├── libsystemd-network
│   ├── arp-util.c
│   ├── arp-util.h
│   ├── dhcp-client-id-internal.h
│   ├── dhcp-client-internal.h
│   ├── dhcp-duid-internal.h
│   ├── dhcp-lease-internal.h
│   ├── dhcp-network.c
│   ├── dhcp-network.h
│   ├── dhcp-option.c
│   ├── dhcp-option.h
│   ├── dhcp-packet.c
│   ├── dhcp-packet.h
│   ├── dhcp-protocol.h
│   ├── dhcp-server-internal.h
│   ├── dhcp-server-lease-internal.h
│   ├── dhcp6-client-internal.h
│   ├── dhcp6-internal.h
│   ├── dhcp6-lease-internal.h
│   ├── dhcp6-network.c
│   ├── dhcp6-option.c
│   ├── dhcp6-option.h
│   ├── dhcp6-protocol.c
│   ├── dhcp6-protocol.h
│   ├── dns-resolver-internal.h
│   ├── fuzz-dhcp-client.c
│   ├── fuzz-dhcp-server-relay.c
│   ├── fuzz-dhcp-server.c
│   ├── fuzz-dhcp6-client.c
│   ├── fuzz-dhcp6-client.options
│   ├── fuzz-lldp-rx.c
│   ├── fuzz-lldp-rx.options
│   ├── fuzz-ndisc-rs.c
│   ├── fuzz-ndisc-rs.options
│   ├── icmp6-packet.c
│   ├── icmp6-packet.h
│   ├── icmp6-test-util.c
│   ├── icmp6-test-util.h
│   ├── icmp6-util.c
│   ├── icmp6-util.h
│   ├── lldp-neighbor.c
│   ├── lldp-neighbor.h
│   ├── lldp-network.c
│   ├── lldp-network.h
│   ├── lldp-rx-internal.h
│   ├── meson.build
│   ├── ndisc-internal.h
│   ├── ndisc-neighbor-internal.h
│   ├── ndisc-option.c
│   ├── ndisc-option.h
│   ├── ndisc-redirect-internal.h
│   ├── ndisc-router-internal.h
│   ├── ndisc-router-solicit-internal.h
│   ├── network-common.c
│   ├── network-common.h
│   ├── network-internal.c
│   ├── network-internal.h
│   ├── radv-internal.h
│   ├── sd-dhcp-client-id.c
│   ├── sd-dhcp-client.c
│   ├── sd-dhcp-duid.c
│   ├── sd-dhcp-lease.c
│   ├── sd-dhcp-server-lease.c
│   ├── sd-dhcp-server.c
│   ├── sd-dhcp6-client.c
│   ├── sd-dhcp6-lease.c
│   ├── sd-dns-resolver.c
│   ├── sd-dns-resolver.h
│   ├── sd-ipv4acd.c
│   ├── sd-ipv4ll.c
│   ├── sd-lldp-rx.c
│   ├── sd-lldp-tx.c
│   ├── sd-ndisc-neighbor.c
│   ├── sd-ndisc-redirect.c
│   ├── sd-ndisc-router-solicit.c
│   ├── sd-ndisc-router.c
│   ├── sd-ndisc.c
│   ├── sd-radv.c
│   ├── test-acd.c
│   ├── test-dhcp-client.c
│   ├── test-dhcp-option.c
│   ├── test-dhcp-server.c
│   ├── test-dhcp6-client.c
│   ├── test-ipv4ll-manual.c
│   ├── test-ipv4ll.c
│   ├── test-lldp-rx.c
│   ├── test-ndisc-ra.c
│   ├── test-ndisc-rs.c
│   ├── test-ndisc-send.c
│   └── test-sd-dhcp-lease.c
├── libudev                         # XXX: Used by udev
│   ├── libudev-device-internal.h
│   ├── libudev-device.c
│   ├── libudev-enumerate.c
│   ├── libudev-hwdb.c
│   ├── libudev-list-internal.h
│   ├── libudev-list.c
│   ├── libudev-monitor.c
│   ├── libudev-queue.c
│   ├── libudev-util.c
│   ├── libudev-util.h
│   ├── libudev.c
│   ├── libudev.h
│   ├── libudev.pc.in
│   ├── libudev.sym
│   ├── meson.build
│   ├── test-libudev.c
│   └── test-udev-device-thread.c
├── locale
│   ├── kbd-model-map
│   ├── language-fallback-map
│   ├── localectl.c
│   ├── localed-util.c
│   ├── localed-util.h
│   ├── localed.c
│   ├── meson.build
│   ├── org.freedesktop.locale1.conf
│   ├── org.freedesktop.locale1.policy
│   ├── org.freedesktop.locale1.service
│   ├── test-localed-util.c
│   ├── xkbcommon-util.c
│   └── xkbcommon-util.h
├── login
│   ├── 10-systemd-logind-root-ignore-inhibitors.rules.example
│   ├── inhibit.c
│   ├── loginctl.c
│   ├── logind-action.c
│   ├── logind-action.h
│   ├── logind-brightness.c
│   ├── logind-brightness.h
│   ├── logind-button.c
│   ├── logind-button.h
│   ├── logind-core.c
│   ├── logind-dbus.c
│   ├── logind-dbus.h
│   ├── logind-device.c
│   ├── logind-device.h
│   ├── logind-forward.h
│   ├── logind-gperf.gperf
│   ├── logind-inhibit.c
│   ├── logind-inhibit.h
│   ├── logind-polkit.c
│   ├── logind-polkit.h
│   ├── logind-seat-dbus.c
│   ├── logind-seat-dbus.h
│   ├── logind-seat.c
│   ├── logind-seat.h
│   ├── logind-session-dbus.c
│   ├── logind-session-dbus.h
│   ├── logind-session-device.c
│   ├── logind-session-device.h
│   ├── logind-session.c
│   ├── logind-session.h
│   ├── logind-user-dbus.c
│   ├── logind-user-dbus.h
│   ├── logind-user.c
│   ├── logind-user.h
│   ├── logind-utmp.c
│   ├── logind-utmp.h
│   ├── logind-varlink.c
│   ├── logind-varlink.h
│   ├── logind-wall.c
│   ├── logind.c
│   ├── logind.conf.in
│   ├── logind.h
│   ├── meson.build
│   ├── org.freedesktop.login1.conf
│   ├── org.freedesktop.login1.policy
│   ├── org.freedesktop.login1.service
│   ├── pam_systemd_loadkey.c
│   ├── pam_systemd_loadkey.sym
│   ├── pam_systemd.c
│   ├── pam_systemd.sym
│   ├── sysfs-show.c
│   ├── sysfs-show.h
│   ├── systemd-user.in
│   ├── test-inhibit.c
│   ├── test-login-shared.c
│   ├── test-login-tables.c
│   ├── test-session-properties.c
│   └── user-runtime-dir.c
├── machine
│   ├── image-dbus.c
│   ├── image-dbus.h
│   ├── image-varlink.c
│   ├── image-varlink.h
│   ├── image.c
│   ├── image.h
│   ├── machine-dbus.c
│   ├── machine-dbus.h
│   ├── machine-forward.h
│   ├── machine-varlink.c
│   ├── machine-varlink.h
│   ├── machine.c
│   ├── machine.h
│   ├── machinectl.c
│   ├── machined-core.c
│   ├── machined-dbus.c
│   ├── machined-varlink.c
│   ├── machined-varlink.h
│   ├── machined.c
│   ├── machined.h
│   ├── meson.build
│   ├── operation.c
│   ├── operation.h
│   ├── org.freedesktop.machine1.conf
│   ├── org.freedesktop.machine1.policy
│   ├── org.freedesktop.machine1.service
│   └── test-machine-tables.c
├── machine-id-setup
│   ├── machine-id-setup-main.c
│   └── meson.build
├── measure
│   ├── measure-tool.c
│   └── meson.build
├── modules-load
│   ├── meson.build
│   └── modules-load.c
├── mount
│   ├── meson.build
│   └── mount-tool.c
├── mountfsd
│   ├── io.systemd.mount-file-system.policy
│   ├── meson.build
│   ├── mountfsd-manager.c
│   ├── mountfsd-manager.h
│   ├── mountfsd.c
│   └── mountwork.c
├── network
│   ├── bpf
│   │   └── sysctl-monitor
│   │       ├── meson.build
│   │       ├── sysctl-monitor-skel.h
│   │       ├── sysctl-monitor.bpf.c
│   │       └── sysctl-write-event.h
│   ├── fuzz-netdev-parser.c
│   ├── fuzz-netdev-parser.options
│   ├── fuzz-network-parser.c
│   ├── fuzz-network-parser.options
│   ├── generator
│   │   ├── network-generator-main.c
│   │   ├── network-generator.c
│   │   ├── network-generator.h
│   │   └── test-network-generator.c
│   ├── meson.build
│   ├── netdev
│   │   ├── bareudp.c
│   │   ├── bareudp.h
│   │   ├── batadv.c
│   │   ├── batadv.h
│   │   ├── bond.c
│   │   ├── bond.h
│   │   ├── bridge.c
│   │   ├── bridge.h
│   │   ├── dummy.c
│   │   ├── dummy.h
│   │   ├── fou-tunnel.c
│   │   ├── fou-tunnel.h
│   │   ├── geneve.c
│   │   ├── geneve.h
│   │   ├── hsr.c
│   │   ├── hsr.h
│   │   ├── ifb.c
│   │   ├── ifb.h
│   │   ├── ipoib.c
│   │   ├── ipoib.h
│   │   ├── ipvlan.c
│   │   ├── ipvlan.h
│   │   ├── l2tp-tunnel.c
│   │   ├── l2tp-tunnel.h
│   │   ├── macsec.c
│   │   ├── macsec.h
│   │   ├── macvlan.c
│   │   ├── macvlan.h
│   │   ├── netdev-gperf.gperf
│   │   ├── netdev-util.c
│   │   ├── netdev-util.h
│   │   ├── netdev.c
│   │   ├── netdev.h
│   │   ├── nlmon.c
│   │   ├── nlmon.h
│   │   ├── tunnel.c
│   │   ├── tunnel.h
│   │   ├── tuntap.c
│   │   ├── tuntap.h
│   │   ├── vcan.c
│   │   ├── vcan.h
│   │   ├── veth.c
│   │   ├── veth.h
│   │   ├── vlan.c
│   │   ├── vlan.h
│   │   ├── vrf.c
│   │   ├── vrf.h
│   │   ├── vxcan.c
│   │   ├── vxcan.h
│   │   ├── vxlan.c
│   │   ├── vxlan.h
│   │   ├── wireguard.c
│   │   ├── wireguard.h
│   │   ├── wlan.c
│   │   ├── wlan.h
│   │   ├── xfrm.c
│   │   └── xfrm.h
│   ├── networkctl-address-label.c
│   ├── networkctl-address-label.h
│   ├── networkctl-config-file.c
│   ├── networkctl-config-file.h
│   ├── networkctl-description.c
│   ├── networkctl-description.h
│   ├── networkctl-dump-util.c
│   ├── networkctl-dump-util.h
│   ├── networkctl-journal.c
│   ├── networkctl-journal.h
│   ├── networkctl-link-info.c
│   ├── networkctl-link-info.h
│   ├── networkctl-list.c
│   ├── networkctl-list.h
│   ├── networkctl-lldp.c
│   ├── networkctl-lldp.h
│   ├── networkctl-misc.c
│   ├── networkctl-misc.h
│   ├── networkctl-status-link.c
│   ├── networkctl-status-link.h
│   ├── networkctl-status-system.c
│   ├── networkctl-status-system.h
│   ├── networkctl-util.c
│   ├── networkctl-util.h
│   ├── networkctl.c
│   ├── networkctl.h
│   ├── networkd-address-generation.c
│   ├── networkd-address-generation.h
│   ├── networkd-address-label.c
│   ├── networkd-address-label.h
│   ├── networkd-address-pool.c
│   ├── networkd-address-pool.h
│   ├── networkd-address.c
│   ├── networkd-address.h
│   ├── networkd-bridge-fdb.c
│   ├── networkd-bridge-fdb.h
│   ├── networkd-bridge-mdb.c
│   ├── networkd-bridge-mdb.h
│   ├── networkd-bridge-vlan.c
│   ├── networkd-bridge-vlan.h
│   ├── networkd-can.c
│   ├── networkd-can.h
│   ├── networkd-conf.c
│   ├── networkd-conf.h
│   ├── networkd-dhcp-common.c
│   ├── networkd-dhcp-common.h
│   ├── networkd-dhcp-prefix-delegation.c
│   ├── networkd-dhcp-prefix-delegation.h
│   ├── networkd-dhcp-server-bus.c
│   ├── networkd-dhcp-server-bus.h
│   ├── networkd-dhcp-server-static-lease.c
│   ├── networkd-dhcp-server-static-lease.h
│   ├── networkd-dhcp-server.c
│   ├── networkd-dhcp-server.h
│   ├── networkd-dhcp4-bus.c
│   ├── networkd-dhcp4-bus.h
│   ├── networkd-dhcp4.c
│   ├── networkd-dhcp4.h
│   ├── networkd-dhcp6-bus.c
│   ├── networkd-dhcp6-bus.h
│   ├── networkd-dhcp6.c
│   ├── networkd-dhcp6.h
│   ├── networkd-dns.c
│   ├── networkd-dns.h
│   ├── networkd-forward.h
│   ├── networkd-gperf.gperf
│   ├── networkd-ipv4acd.c
│   ├── networkd-ipv4acd.h
│   ├── networkd-ipv4ll.c
│   ├── networkd-ipv4ll.h
│   ├── networkd-ipv6-proxy-ndp.c
│   ├── networkd-ipv6-proxy-ndp.h
│   ├── networkd-ipv6ll.c
│   ├── networkd-ipv6ll.h
│   ├── networkd-json.c
│   ├── networkd-json.h
│   ├── networkd-link-bus.c
│   ├── networkd-link-bus.h
│   ├── networkd-link.c
│   ├── networkd-link.h
│   ├── networkd-lldp-rx.c
│   ├── networkd-lldp-rx.h
│   ├── networkd-lldp-tx.c
│   ├── networkd-lldp-tx.h
│   ├── networkd-manager-bus.c
│   ├── networkd-manager-bus.h
│   ├── networkd-manager-varlink.c
│   ├── networkd-manager-varlink.h
│   ├── networkd-manager.c
│   ├── networkd-manager.h
│   ├── networkd-ndisc.c
│   ├── networkd-ndisc.h
│   ├── networkd-neighbor.c
│   ├── networkd-neighbor.h
│   ├── networkd-netlabel.c
│   ├── networkd-netlabel.h
│   ├── networkd-network-bus.c
│   ├── networkd-network-bus.h
│   ├── networkd-network-gperf.gperf
│   ├── networkd-network.c
│   ├── networkd-network.h
│   ├── networkd-nexthop.c
│   ├── networkd-nexthop.h
│   ├── networkd-ntp.c
│   ├── networkd-ntp.h
│   ├── networkd-queue.c
│   ├── networkd-queue.h
│   ├── networkd-radv.c
│   ├── networkd-radv.h
│   ├── networkd-route-metric.c
│   ├── networkd-route-metric.h
│   ├── networkd-route-nexthop.c
│   ├── networkd-route-nexthop.h
│   ├── networkd-route-util.c
│   ├── networkd-route-util.h
│   ├── networkd-route.c
│   ├── networkd-route.h
│   ├── networkd-routing-policy-rule.c
│   ├── networkd-routing-policy-rule.h
│   ├── networkd-serialize.c
│   ├── networkd-serialize.h
│   ├── networkd-setlink.c
│   ├── networkd-setlink.h
│   ├── networkd-speed-meter.c
│   ├── networkd-speed-meter.h
│   ├── networkd-sriov.c
│   ├── networkd-sriov.h
│   ├── networkd-state-file.c
│   ├── networkd-state-file.h
│   ├── networkd-sysctl.c
│   ├── networkd-sysctl.h
│   ├── networkd-util.c
│   ├── networkd-util.h
│   ├── networkd-wifi.c
│   ├── networkd-wifi.h
│   ├── networkd-wiphy.c
│   ├── networkd-wiphy.h
│   ├── networkd.c
│   ├── networkd.conf
│   ├── org.freedesktop.network1.conf
│   ├── org.freedesktop.network1.policy
│   ├── org.freedesktop.network1.service
│   ├── systemd-networkd.pkla
│   ├── systemd-networkd.rules
│   ├── tc
│   │   ├── cake.c
│   │   ├── cake.h
│   │   ├── codel.c
│   │   ├── codel.h
│   │   ├── drr.c
│   │   ├── drr.h
│   │   ├── ets.c
│   │   ├── ets.h
│   │   ├── fifo.c
│   │   ├── fifo.h
│   │   ├── fq-codel.c
│   │   ├── fq-codel.h
│   │   ├── fq-pie.c
│   │   ├── fq-pie.h
│   │   ├── fq.c
│   │   ├── fq.h
│   │   ├── gred.c
│   │   ├── gred.h
│   │   ├── hhf.c
│   │   ├── hhf.h
│   │   ├── htb.c
│   │   ├── htb.h
│   │   ├── mq.c
│   │   ├── mq.h
│   │   ├── multiq.c
│   │   ├── multiq.h
│   │   ├── netem.c
│   │   ├── netem.h
│   │   ├── pie.c
│   │   ├── pie.h
│   │   ├── qdisc.c
│   │   ├── qdisc.h
│   │   ├── qfq.c
│   │   ├── qfq.h
│   │   ├── sfb.c
│   │   ├── sfb.h
│   │   ├── sfq.c
│   │   ├── sfq.h
│   │   ├── tbf.c
│   │   ├── tbf.h
│   │   ├── tc-util.c
│   │   ├── tc-util.h
│   │   ├── tc.c
│   │   ├── tc.h
│   │   ├── tclass.c
│   │   ├── tclass.h
│   │   ├── teql.c
│   │   └── teql.h
│   ├── test-network-tables.c
│   ├── test-network.c
│   ├── test-networkd-address.c
│   ├── test-networkd-conf.c
│   ├── test-networkd-util.c
│   └── wait-online
│       ├── dns-configuration.c
│       ├── dns-configuration.h
│       ├── wait-online-link.c
│       ├── wait-online-link.h
│       ├── wait-online-manager.c
│       ├── wait-online-manager.h
│       └── wait-online.c
├── NOTES.md
├── notify
│   ├── meson.build
│   └── notify.c
├── nspawn
│   ├── fuzz-nspawn-oci.c
│   ├── fuzz-nspawn-oci.options
│   ├── fuzz-nspawn-settings.c
│   ├── fuzz-nspawn-settings.options
│   ├── meson.build
│   ├── nspawn-bind-user.c
│   ├── nspawn-bind-user.h
│   ├── nspawn-cgroup.c
│   ├── nspawn-cgroup.h
│   ├── nspawn-expose-ports.c
│   ├── nspawn-expose-ports.h
│   ├── nspawn-gperf.gperf
│   ├── nspawn-mount.c
│   ├── nspawn-mount.h
│   ├── nspawn-network.c
│   ├── nspawn-network.h
│   ├── nspawn-oci.c
│   ├── nspawn-oci.h
│   ├── nspawn-register.c
│   ├── nspawn-register.h
│   ├── nspawn-seccomp.c
│   ├── nspawn-seccomp.h
│   ├── nspawn-settings.c
│   ├── nspawn-settings.h
│   ├── nspawn-setuid.c
│   ├── nspawn-setuid.h
│   ├── nspawn-stub-pid1.c
│   ├── nspawn-stub-pid1.h
│   ├── nspawn.c
│   ├── nspawn.h
│   └── test-nspawn-tables.c
├── nsresourced
│   ├── bpf
│   │   └── userns-restrict
│   │       ├── meson.build
│   │       ├── userns-restrict-skel.h
│   │       └── userns-restrict.bpf.c
│   ├── io.systemd.namespace-resource.policy
│   ├── meson.build
│   ├── nsresourced-manager.c
│   ├── nsresourced-manager.h
│   ├── nsresourced.c
│   ├── nsresourcework.c
│   ├── test-userns-restrict.c
│   ├── userns-registry.c
│   ├── userns-registry.h
│   ├── userns-restrict.c
│   └── userns-restrict.h
├── nss-myhostname
│   ├── meson.build
│   ├── nss-myhostname.c
│   └── nss-myhostname.sym
├── nss-mymachines
│   ├── meson.build
│   ├── nss-mymachines.c
│   └── nss-mymachines.sym
├── nss-resolve
│   ├── meson.build
│   ├── nss-resolve.c
│   └── nss-resolve.sym
├── nss-systemd
│   ├── meson.build
│   ├── nss-systemd.c
│   ├── nss-systemd.h
│   ├── nss-systemd.sym
│   ├── userdb-glue.c
│   └── userdb-glue.h
├── oom
│   ├── meson.build
│   ├── oomctl.c
│   ├── oomd-conf.c
│   ├── oomd-conf.h
│   ├── oomd-manager-bus.c
│   ├── oomd-manager-bus.h
│   ├── oomd-manager.c
│   ├── oomd-manager.h
│   ├── oomd-util.c
│   ├── oomd-util.h
│   ├── oomd.c
│   ├── oomd.conf
│   ├── org.freedesktop.oom1.conf
│   ├── org.freedesktop.oom1.service
│   └── test-oomd-util.c
├── path
│   ├── meson.build
│   └── path-tool.c
├── pcrextend
│   ├── meson.build
│   └── pcrextend.c
├── pcrlock
│   ├── meson.build
│   ├── pcrlock-firmware.c
│   ├── pcrlock-firmware.h
│   ├── pcrlock.c
│   └── pcrlock.d
│       ├── 350-action-efi-application.pcrlock
│       ├── 400-secureboot-separator.pcrlock.d
│       │   ├── 300-0x00000000.pcrlock
│       │   └── 600-0xffffffff.pcrlock
│       ├── 500-separator.pcrlock.d
│       │   ├── 300-0x00000000.pcrlock
│       │   └── 600-0xffffffff.pcrlock
│       ├── 700-action-efi-exit-boot-services.pcrlock.d
│       │   ├── 300-present.pcrlock
│       │   └── 600-absent.pcrlock
│       ├── 750-enter-initrd.pcrlock
│       ├── 800-leave-initrd.pcrlock
│       ├── 850-sysinit.pcrlock
│       ├── 900-ready.pcrlock
│       ├── 950-shutdown.pcrlock
│       └── 990-final.pcrlock
├── portable
│   ├── meson.build
│   ├── org.freedesktop.portable1.conf
│   ├── org.freedesktop.portable1.policy
│   ├── org.freedesktop.portable1.service
│   ├── portable.c
│   ├── portable.h
│   ├── portablectl.c
│   ├── portabled-bus.c
│   ├── portabled-bus.h
│   ├── portabled-forward.h
│   ├── portabled-image-bus.c
│   ├── portabled-image-bus.h
│   ├── portabled-image.c
│   ├── portabled-image.h
│   ├── portabled-operation.c
│   ├── portabled-operation.h
│   ├── portabled.c
│   ├── portabled.h
│   └── profile
│       ├── default
│       │   └── service.conf
│       ├── nonetwork
│       │   └── service.conf
│       ├── strict
│       │   └── service.conf
│       └── trusted
│           └── service.conf
├── pstore
│   ├── meson.build
│   ├── pstore.c
│   └── pstore.conf
├── ptyfwd
│   ├── meson.build
│   └── ptyfwd-tool.c
├── quotacheck
│   ├── meson.build
│   └── quotacheck.c
├── random-seed
│   ├── meson.build
│   └── random-seed-tool.c
├── rc-local-generator
│   ├── meson.build
│   └── rc-local-generator.c
├── remount-fs
│   ├── meson.build
│   └── remount-fs.c
├── repart
│   ├── definitions
│   │   ├── confext.repart.d
│   │   │   ├── 10-root.conf
│   │   │   ├── 20-root-verity.conf
│   │   │   └── 30-root-verity-sig.conf
│   │   ├── portable.repart.d
│   │   │   ├── 10-root.conf
│   │   │   ├── 20-root-verity.conf
│   │   │   └── 30-root-verity-sig.conf
│   │   └── sysext.repart.d
│   │       ├── 10-root.conf
│   │       ├── 20-root-verity.conf
│   │       └── 30-root-verity-sig.conf
│   ├── meson.build
│   └── repart.c
├── reply-password
│   ├── meson.build
│   └── reply-password.c
├── resolve
│   ├── dns_type-to-name.awk
│   ├── dns-type.c
│   ├── dns-type.h
│   ├── fuzz-dns-packet.c
│   ├── fuzz-dns-packet.options
│   ├── fuzz-etc-hosts.c
│   ├── fuzz-resource-record.c
│   ├── generate-dns_type-gperf.py
│   ├── generate-dns_type-list.sed
│   ├── meson.build
│   ├── org.freedesktop.resolve1.conf
│   ├── org.freedesktop.resolve1.policy
│   ├── org.freedesktop.resolve1.service
│   ├── resolv.conf
│   ├── resolvconf-compat.c
│   ├── resolvconf-compat.h
│   ├── resolvectl.c
│   ├── resolvectl.h
│   ├── resolved-bus.c
│   ├── resolved-bus.h
│   ├── resolved-conf.c
│   ├── resolved-conf.h
│   ├── resolved-def.h
│   ├── resolved-dns-answer.c
│   ├── resolved-dns-answer.h
│   ├── resolved-dns-cache.c
│   ├── resolved-dns-cache.h
│   ├── resolved-dns-delegate-bus.c
│   ├── resolved-dns-delegate-bus.h
│   ├── resolved-dns-delegate-gperf.gperf
│   ├── resolved-dns-delegate.c
│   ├── resolved-dns-delegate.h
│   ├── resolved-dns-dnssec.c
│   ├── resolved-dns-dnssec.h
│   ├── resolved-dns-packet.c
│   ├── resolved-dns-packet.h
│   ├── resolved-dns-query.c
│   ├── resolved-dns-query.h
│   ├── resolved-dns-question.c
│   ├── resolved-dns-question.h
│   ├── resolved-dns-rr.c
│   ├── resolved-dns-rr.h
│   ├── resolved-dns-scope.c
│   ├── resolved-dns-scope.h
│   ├── resolved-dns-search-domain.c
│   ├── resolved-dns-search-domain.h
│   ├── resolved-dns-server.c
│   ├── resolved-dns-server.h
│   ├── resolved-dns-stream.c
│   ├── resolved-dns-stream.h
│   ├── resolved-dns-stub.c
│   ├── resolved-dns-stub.h
│   ├── resolved-dns-synthesize.c
│   ├── resolved-dns-synthesize.h
│   ├── resolved-dns-transaction.c
│   ├── resolved-dns-transaction.h
│   ├── resolved-dns-trust-anchor.c
│   ├── resolved-dns-trust-anchor.h
│   ├── resolved-dns-zone.c
│   ├── resolved-dns-zone.h
│   ├── resolved-dnssd-bus.c
│   ├── resolved-dnssd-bus.h
│   ├── resolved-dnssd-gperf.gperf
│   ├── resolved-dnssd.c
│   ├── resolved-dnssd.h
│   ├── resolved-dnstls.c
│   ├── resolved-dnstls.h
│   ├── resolved-etc-hosts.c
│   ├── resolved-etc-hosts.h
│   ├── resolved-forward.h
│   ├── resolved-gperf.gperf
│   ├── resolved-link-bus.c
│   ├── resolved-link-bus.h
│   ├── resolved-link.c
│   ├── resolved-link.h
│   ├── resolved-llmnr.c
│   ├── resolved-llmnr.h
│   ├── resolved-manager.c
│   ├── resolved-manager.h
│   ├── resolved-mdns.c
│   ├── resolved-mdns.h
│   ├── resolved-resolv-conf.c
│   ├── resolved-resolv-conf.h
│   ├── resolved-socket-graveyard.c
│   ├── resolved-socket-graveyard.h
│   ├── resolved-timeouts.h
│   ├── resolved-util.c
│   ├── resolved-util.h
│   ├── resolved-varlink.c
│   ├── resolved-varlink.h
│   ├── resolved.c
│   ├── resolved.conf.in
│   ├── RFCs
│   ├── test-dns-answer.c
│   ├── test-dns-cache.c
│   ├── test-dns-packet-append.c
│   ├── test-dns-packet-extract.c
│   ├── test-dns-packet.c
│   ├── test-dns-query.c
│   ├── test-dns-question.c
│   ├── test-dns-rr.c
│   ├── test-dns-search-domain.c
│   ├── test-dns-synthesize.c
│   ├── test-dns-zone.c
│   ├── test-dnssec-complex.c
│   ├── test-dnssec.c
│   ├── test-resolve-tables.c
│   ├── test-resolved-dummy-server.c
│   ├── test-resolved-etc-hosts.c
│   ├── test-resolved-link.c
│   ├── test-resolved-packet.c
│   └── test-resolved-stream.c
├── rfkill
│   ├── meson.build
│   └── rfkill.c
├── rpm
│   ├── macros.systemd.in
│   ├── meson.build
│   ├── systemd-update-helper.in
│   ├── triggers.systemd.in
│   └── triggers.systemd.sh.in
├── run
│   ├── meson.build
│   ├── run.c
│   └── systemd-run0.in
├── run-generator
│   ├── meson.build
│   └── run-generator.c
├── sbsign
│   ├── authenticode.h
│   ├── meson.build
│   └── sbsign.c
├── shared
│   ├── acl-util.c
│   ├── acl-util.h
│   ├── acpi-fpdt.c
│   ├── acpi-fpdt.h
│   ├── apparmor-util.c
│   ├── apparmor-util.h
│   ├── ask-password-agent.c
│   ├── ask-password-agent.h
│   ├── ask-password-api.c
│   ├── ask-password-api.h
│   ├── async.c
│   ├── async.h
│   ├── barrier.c
│   ├── barrier.h
│   ├── base-filesystem.c
│   ├── base-filesystem.h
│   ├── battery-util.c
│   ├── battery-util.h
│   ├── binfmt-util.c
│   ├── binfmt-util.h
│   ├── bitmap.c
│   ├── bitmap.h
│   ├── blkid-util.c
│   ├── blkid-util.h
│   ├── blockdev-list.c
│   ├── blockdev-list.h
│   ├── blockdev-util.c
│   ├── blockdev-util.h
│   ├── bond-util.c
│   ├── bond-util.h
│   ├── boot-entry.c
│   ├── boot-entry.h
│   ├── boot-timestamps.c
│   ├── boot-timestamps.h
│   ├── bootspec.c
│   ├── bootspec.h
│   ├── bpf-compat.h
│   ├── bpf-dlopen.c
│   ├── bpf-dlopen.h
│   ├── bpf-link.c
│   ├── bpf-link.h
│   ├── bpf-program.c
│   ├── bpf-program.h
│   ├── bridge-util.c
│   ├── bridge-util.h
│   ├── btrfs-util.c
│   ├── btrfs-util.h
│   ├── bus-get-properties.c
│   ├── bus-get-properties.h
│   ├── bus-locator.c
│   ├── bus-locator.h
│   ├── bus-log-control-api.c
│   ├── bus-log-control-api.h
│   ├── bus-map-properties.c
│   ├── bus-map-properties.h
│   ├── bus-message-util.c
│   ├── bus-message-util.h
│   ├── bus-object.c
│   ├── bus-object.h
│   ├── bus-polkit.c
│   ├── bus-polkit.h
│   ├── bus-print-properties.c
│   ├── bus-print-properties.h
│   ├── bus-unit-procs.c
│   ├── bus-unit-procs.h
│   ├── bus-unit-util.c
│   ├── bus-unit-util.h
│   ├── bus-util.c
│   ├── bus-util.h
│   ├── bus-wait-for-jobs.c
│   ├── bus-wait-for-jobs.h
│   ├── bus-wait-for-units.c
│   ├── bus-wait-for-units.h
│   ├── calendarspec.c
│   ├── calendarspec.h
│   ├── cgroup-setup.c
│   ├── cgroup-setup.h
│   ├── cgroup-show.c
│   ├── cgroup-show.h
│   ├── chown-recursive.c
│   ├── chown-recursive.h
│   ├── clean-ipc.c
│   ├── clean-ipc.h
│   ├── clock-util.c
│   ├── clock-util.h
│   ├── color-util.c
│   ├── color-util.h
│   ├── common-signal.c
│   ├── common-signal.h
│   ├── compare-operator.c
│   ├── compare-operator.h
│   ├── condition.c
│   ├── condition.h
│   ├── conf-parser-forward.h
│   ├── conf-parser.c
│   ├── conf-parser.h
│   ├── copy.c
│   ├── copy.h
│   ├── coredump-util.c
│   ├── coredump-util.h
│   ├── cpu-set-util.c
│   ├── cpu-set-util.h
│   ├── creds-util.c
│   ├── creds-util.h
│   ├── cryptsetup-fido2.c
│   ├── cryptsetup-fido2.h
│   ├── cryptsetup-tpm2.c
│   ├── cryptsetup-tpm2.h
│   ├── cryptsetup-util.c
│   ├── cryptsetup-util.h
│   ├── daemon-util.c
│   ├── daemon-util.h
│   ├── data-fd-util.c
│   ├── data-fd-util.h
│   ├── dev-setup.c
│   ├── dev-setup.h
│   ├── device-nodes.c
│   ├── device-nodes.h
│   ├── discover-image.c
│   ├── discover-image.h
│   ├── dissect-image.c
│   ├── dissect-image.h
│   ├── dm-util.c
│   ├── dm-util.h
│   ├── dns-domain.c
│   ├── dns-domain.h
│   ├── dropin.c
│   ├── dropin.h
│   ├── edit-util.c
│   ├── edit-util.h
│   ├── efi-api.c
│   ├── efi-api.h
│   ├── efi-loader.c
│   ├── efi-loader.h
│   ├── elf-util.c
│   ├── elf-util.h
│   ├── enable-mempool.c
│   ├── env-file-label.c
│   ├── ethtool-link-mode.py
│   ├── ethtool-util.c
│   ├── ethtool-util.h
│   ├── exec-util.c
│   ├── exec-util.h
│   ├── exit-status.c
│   ├── exit-status.h
│   ├── extension-util.c
│   ├── extension-util.h
│   ├── factory-reset.c
│   ├── factory-reset.h
│   ├── fdisk-util.c
│   ├── fdisk-util.h
│   ├── fdset.c
│   ├── fdset.h
│   ├── fido2-util.c
│   ├── fido2-util.h
│   ├── find-esp.c
│   ├── find-esp.h
│   ├── firewall-util-iptables.c
│   ├── firewall-util-nft.c
│   ├── firewall-util-private.h
│   ├── firewall-util.c
│   ├── firewall-util.h
│   ├── fork-notify.c
│   ├── fork-notify.h
│   ├── format-table.c
│   ├── format-table.h
│   ├── fsck-util.h
│   ├── fstab-util.c
│   ├── fstab-util.h
│   ├── generate-ip-protocol-list.sh
│   ├── generate-syscall-list.py
│   ├── generator.c
│   ├── generator.h
│   ├── geneve-util.c
│   ├── geneve-util.h
│   ├── gpt.c
│   ├── gpt.h
│   ├── group-record.c
│   ├── group-record.h
│   ├── hibernate-util.c
│   ├── hibernate-util.h
│   ├── hostname-setup.c
│   ├── hostname-setup.h
│   ├── hwdb-util.c
│   ├── hwdb-util.h
│   ├── id128-print.c
│   ├── id128-print.h
│   ├── idn-util.c
│   ├── idn-util.h
│   ├── ima-util.c
│   ├── ima-util.h
│   ├── image-policy.c
│   ├── image-policy.h
│   ├── import-util.c
│   ├── import-util.h
│   ├── in-addr-prefix-util.c
│   ├── in-addr-prefix-util.h
│   ├── install-file.c
│   ├── install-file.h
│   ├── install-printf.c
│   ├── install-printf.h
│   ├── install.c
│   ├── install.h
│   ├── ioprio-util.c
│   ├── ioprio-util.h
│   ├── ip-protocol-list.c
│   ├── ip-protocol-list.h
│   ├── ip-protocol-to-name.awk
│   ├── ipvlan-util.c
│   ├── ipvlan-util.h
│   ├── journal-file-util.c
│   ├── journal-file-util.h
│   ├── journal-importer.c
│   ├── journal-importer.h
│   ├── journal-util.c
│   ├── journal-util.h
│   ├── kbd-util.c
│   ├── kbd-util.h
│   ├── kernel-config.c
│   ├── kernel-config.h
│   ├── kernel-image.c
│   ├── kernel-image.h
│   ├── killall.c
│   ├── killall.h
│   ├── label-util.c
│   ├── label-util.h
│   ├── libarchive-util.c
│   ├── libarchive-util.h
│   ├── libaudit-util.c
│   ├── libaudit-util.h
│   ├── libcrypt-util.c
│   ├── libcrypt-util.h
│   ├── libfido2-util.c
│   ├── libfido2-util.h
│   ├── libmount-util.c
│   ├── libmount-util.h
│   ├── libshared.sym
│   ├── local-addresses.c
│   ├── local-addresses.h
│   ├── locale-setup.c
│   ├── locale-setup.h
│   ├── log-link.h
│   ├── logs-show.c
│   ├── logs-show.h
│   ├── loop-util.c
│   ├── loop-util.h
│   ├── loopback-setup.c
│   ├── loopback-setup.h
│   ├── lsm-util.c
│   ├── lsm-util.h
│   ├── machine-bind-user.c
│   ├── machine-bind-user.h
│   ├── machine-credential.c
│   ├── machine-credential.h
│   ├── machine-id-setup.c
│   ├── machine-id-setup.h
│   ├── machine-pool.c
│   ├── machine-pool.h
│   ├── macvlan-util.c
│   ├── macvlan-util.h
│   ├── main-func.c
│   ├── main-func.h
│   ├── meson.build
│   ├── mkdir-label.c
│   ├── mkdir-label.h
│   ├── mkfs-util.c
│   ├── mkfs-util.h
│   ├── module-util.c
│   ├── module-util.h
│   ├── mount-setup.c
│   ├── mount-setup.h
│   ├── mount-util.c
│   ├── mount-util.h
│   ├── net-condition.c
│   ├── net-condition.h
│   ├── netif-naming-scheme.c
│   ├── netif-naming-scheme.h
│   ├── netif-sriov.c
│   ├── netif-sriov.h
│   ├── netif-util.c
│   ├── netif-util.h
│   ├── notify-recv.c
│   ├── notify-recv.h
│   ├── nsflags.c
│   ├── nsflags.h
│   ├── nsresource.c
│   ├── nsresource.h
│   ├── numa-util.c
│   ├── numa-util.h
│   ├── open-file.c
│   ├── open-file.h
│   ├── openssl-util.c
│   ├── openssl-util.h
│   ├── osc-context.c
│   ├── osc-context.h
│   ├── output-mode.c
│   ├── output-mode.h
│   ├── pager.c
│   ├── pager.h
│   ├── pam-util.c
│   ├── pam-util.h
│   ├── parse-argument.c
│   ├── parse-argument.h
│   ├── parse-helpers.c
│   ├── parse-helpers.h
│   ├── password-quality-util-passwdqc.c
│   ├── password-quality-util-passwdqc.h
│   ├── password-quality-util-pwquality.c
│   ├── password-quality-util-pwquality.h
│   ├── password-quality-util.h
│   ├── pcre2-util.c
│   ├── pcre2-util.h
│   ├── pcrextend-util.c
│   ├── pcrextend-util.h
│   ├── pe-binary.c
│   ├── pe-binary.h
│   ├── pkcs11-util.c
│   ├── pkcs11-util.h
│   ├── plymouth-util.c
│   ├── plymouth-util.h
│   ├── polkit-agent.c
│   ├── polkit-agent.h
│   ├── portable-util.c
│   ├── portable-util.h
│   ├── pretty-print.c
│   ├── pretty-print.h
│   ├── ptyfwd.c
│   ├── ptyfwd.h
│   ├── qrcode-util.c
│   ├── qrcode-util.h
│   ├── quota-util.c
│   ├── quota-util.h
│   ├── reboot-util.c
│   ├── reboot-util.h
│   ├── recovery-key.c
│   ├── recovery-key.h
│   ├── resize-fs.c
│   ├── resize-fs.h
│   ├── resolve-util.c
│   ├── resolve-util.h
│   ├── rm-rf.c
│   ├── rm-rf.h
│   ├── seccomp-util.c
│   ├── seccomp-util.h
│   ├── securebits-util.c
│   ├── securebits-util.h
│   ├── selinux-util.c
│   ├── selinux-util.h
│   ├── serialize.c
│   ├── serialize.h
│   ├── service-util.c
│   ├── service-util.h
│   ├── shift-uid.c
│   ├── shift-uid.h
│   ├── sleep-config.c
│   ├── sleep-config.h
│   ├── smack-util.c
│   ├── smack-util.h
│   ├── smbios11.c
│   ├── smbios11.h
│   ├── socket-label.c
│   ├── socket-netlink.c
│   ├── socket-netlink.h
│   ├── specifier.c
│   ├── specifier.h
│   ├── switch-root.c
│   ├── switch-root.h
│   ├── test-tables.h
│   ├── tests.c
│   ├── tests.h
│   ├── tmpfile-util-label.c
│   ├── tmpfile-util-label.h
│   ├── tomoyo-util.c
│   ├── tomoyo-util.h
│   ├── tpm2-event-log.c
│   ├── tpm2-event-log.h
│   ├── tpm2-util.c
│   ├── tpm2-util.h
│   ├── udev-util.c
│   ├── udev-util.h
│   ├── unit-file.c
│   ├── unit-file.h
│   ├── user-record-nss.c
│   ├── user-record-nss.h
│   ├── user-record-show.c
│   ├── user-record-show.h
│   ├── user-record.c
│   ├── user-record.h
│   ├── userdb-dropin.c
│   ├── userdb-dropin.h
│   ├── userdb.c
│   ├── userdb.h
│   ├── utmp-wtmp.c
│   ├── utmp-wtmp.h
│   ├── varlink-idl-common.c
│   ├── varlink-idl-common.h
│   ├── varlink-io.systemd.AskPassword.c
│   ├── varlink-io.systemd.AskPassword.h
│   ├── varlink-io.systemd.BootControl.c
│   ├── varlink-io.systemd.BootControl.h
│   ├── varlink-io.systemd.Credentials.c
│   ├── varlink-io.systemd.Credentials.h
│   ├── varlink-io.systemd.FactoryReset.c
│   ├── varlink-io.systemd.FactoryReset.h
│   ├── varlink-io.systemd.Hostname.c
│   ├── varlink-io.systemd.Hostname.h
│   ├── varlink-io.systemd.Import.c
│   ├── varlink-io.systemd.Import.h
│   ├── varlink-io.systemd.Journal.c
│   ├── varlink-io.systemd.Journal.h
│   ├── varlink-io.systemd.Login.c
│   ├── varlink-io.systemd.Login.h
│   ├── varlink-io.systemd.Machine.c
│   ├── varlink-io.systemd.Machine.h
│   ├── varlink-io.systemd.MachineImage.c
│   ├── varlink-io.systemd.MachineImage.h
│   ├── varlink-io.systemd.ManagedOOM.c
│   ├── varlink-io.systemd.ManagedOOM.h
│   ├── varlink-io.systemd.Manager.c
│   ├── varlink-io.systemd.Manager.h
│   ├── varlink-io.systemd.MountFileSystem.c
│   ├── varlink-io.systemd.MountFileSystem.h
│   ├── varlink-io.systemd.NamespaceResource.c
│   ├── varlink-io.systemd.NamespaceResource.h
│   ├── varlink-io.systemd.Network.c
│   ├── varlink-io.systemd.Network.h
│   ├── varlink-io.systemd.oom.c
│   ├── varlink-io.systemd.oom.h
│   ├── varlink-io.systemd.PCRExtend.c
│   ├── varlink-io.systemd.PCRExtend.h
│   ├── varlink-io.systemd.PCRLock.c
│   ├── varlink-io.systemd.PCRLock.h
│   ├── varlink-io.systemd.Resolve.c
│   ├── varlink-io.systemd.Resolve.h
│   ├── varlink-io.systemd.Resolve.Monitor.c
│   ├── varlink-io.systemd.Resolve.Monitor.h
│   ├── varlink-io.systemd.service.c
│   ├── varlink-io.systemd.service.h
│   ├── varlink-io.systemd.sysext.c
│   ├── varlink-io.systemd.sysext.h
│   ├── varlink-io.systemd.Udev.c
│   ├── varlink-io.systemd.Udev.h
│   ├── varlink-io.systemd.Unit.c
│   ├── varlink-io.systemd.Unit.h
│   ├── varlink-io.systemd.UserDatabase.c
│   ├── varlink-io.systemd.UserDatabase.h
│   ├── varlink-serialize.c
│   ├── varlink-serialize.h
│   ├── vconsole-util.c
│   ├── vconsole-util.h
│   ├── verb-log-control.c
│   ├── verb-log-control.h
│   ├── verbs.c
│   ├── verbs.h
│   ├── vlan-util.c
│   ├── vlan-util.h
│   ├── volatile-util.c
│   ├── volatile-util.h
│   ├── vpick.c
│   ├── vpick.h
│   ├── wall.c
│   ├── wall.h
│   ├── watchdog.c
│   ├── watchdog.h
│   ├── web-util.c
│   ├── web-util.h
│   ├── wifi-util.c
│   ├── wifi-util.h
│   ├── xml.c
│   └── xml.h
├── shutdown                # XXX: What magic happens during shutdown
│   ├── detach-dm.c
│   ├── detach-dm.h
│   ├── detach-loopback.c
│   ├── detach-loopback.h
│   ├── detach-md.c
│   ├── detach-md.h
│   ├── detach-swap.c
│   ├── detach-swap.h
│   ├── meson.build
│   ├── shutdown.c
│   ├── shutdown.h
│   ├── test-umount.c
│   ├── umount.c
│   └── umount.h
├── sleep                   # XXX: What magic happens during the sleep
│   ├── battery-capacity.c
│   ├── battery-capacity.h
│   ├── meson.build
│   ├── sleep.c
│   ├── sleep.conf
│   └── test-battery-capacity.c
├── socket-activate
│   ├── meson.build
│   └── socket-activate.c
├── socket-proxy
│   ├── meson.build
│   └── socket-proxyd.c
├── ssh-generator
│   ├── 20-systemd-ssh-proxy.conf.in
│   ├── meson.build
│   ├── ssh-generator.c
│   ├── ssh-issue.c
│   └── ssh-proxy.c
├── stdio-bridge
│   ├── meson.build
│   └── stdio-bridge.c
├── storagetm
│   ├── meson.build
│   └── storagetm.c
├── sulogin-shell
│   ├── meson.build
│   └── sulogin-shell.c
├── sysctl
│   ├── meson.build
│   └── sysctl.c
├── sysext
│   ├── meson.build
│   └── sysext.c
├── system-update-generator
│   ├── meson.build
│   └── system-update-generator.c
├── systemctl
│   ├── fuzz-systemctl-parse-argv.c
│   ├── meson.build
│   ├── systemctl-add-dependency.c
│   ├── systemctl-add-dependency.h
│   ├── systemctl-cancel-job.c
│   ├── systemctl-cancel-job.h
│   ├── systemctl-clean-or-freeze.c
│   ├── systemctl-clean-or-freeze.h
│   ├── systemctl-compat-halt.c
│   ├── systemctl-compat-halt.h
│   ├── systemctl-compat-shutdown.c
│   ├── systemctl-compat-shutdown.h
│   ├── systemctl-daemon-reload.c
│   ├── systemctl-daemon-reload.h
│   ├── systemctl-edit.c
│   ├── systemctl-edit.h
│   ├── systemctl-enable.c
│   ├── systemctl-enable.h
│   ├── systemctl-is-active.c
│   ├── systemctl-is-active.h
│   ├── systemctl-is-enabled.c
│   ├── systemctl-is-enabled.h
│   ├── systemctl-is-system-running.c
│   ├── systemctl-is-system-running.h
│   ├── systemctl-kill.c
│   ├── systemctl-kill.h
│   ├── systemctl-list-dependencies.c
│   ├── systemctl-list-dependencies.h
│   ├── systemctl-list-jobs.c
│   ├── systemctl-list-jobs.h
│   ├── systemctl-list-machines.c
│   ├── systemctl-list-machines.h
│   ├── systemctl-list-unit-files.c
│   ├── systemctl-list-unit-files.h
│   ├── systemctl-list-units.c
│   ├── systemctl-list-units.h
│   ├── systemctl-log-setting.c
│   ├── systemctl-log-setting.h
│   ├── systemctl-logind.c
│   ├── systemctl-logind.h
│   ├── systemctl-main.c
│   ├── systemctl-mount.c
│   ├── systemctl-mount.h
│   ├── systemctl-preset-all.c
│   ├── systemctl-preset-all.h
│   ├── systemctl-reset-failed.c
│   ├── systemctl-reset-failed.h
│   ├── systemctl-service-watchdogs.c
│   ├── systemctl-service-watchdogs.h
│   ├── systemctl-set-default.c
│   ├── systemctl-set-default.h
│   ├── systemctl-set-environment.c
│   ├── systemctl-set-environment.h
│   ├── systemctl-set-property.c
│   ├── systemctl-set-property.h
│   ├── systemctl-show.c
│   ├── systemctl-show.h
│   ├── systemctl-start-special.c
│   ├── systemctl-start-special.h
│   ├── systemctl-start-unit.c
│   ├── systemctl-start-unit.h
│   ├── systemctl-switch-root.c
│   ├── systemctl-switch-root.h
│   ├── systemctl-sysv-compat.c
│   ├── systemctl-sysv-compat.h
│   ├── systemctl-trivial-method.c
│   ├── systemctl-trivial-method.h
│   ├── systemctl-util.c
│   ├── systemctl-util.h
│   ├── systemctl-whoami.c
│   ├── systemctl-whoami.h
│   ├── systemctl.c
│   ├── systemctl.h
│   └── systemd-sysv-install.SKELETON
├── systemd
│   ├── _sd-common.h
│   ├── meson.build
│   ├── sd-bus-protocol.h
│   ├── sd-bus-vtable.h
│   ├── sd-bus.h
│   ├── sd-daemon.h
│   ├── sd-device.h
│   ├── sd-dhcp-client-id.h
│   ├── sd-dhcp-client.h
│   ├── sd-dhcp-duid.h
│   ├── sd-dhcp-lease.h
│   ├── sd-dhcp-option.h
│   ├── sd-dhcp-protocol.h
│   ├── sd-dhcp-server-lease.h
│   ├── sd-dhcp-server.h
│   ├── sd-dhcp6-client.h
│   ├── sd-dhcp6-lease.h
│   ├── sd-dhcp6-option.h
│   ├── sd-dhcp6-protocol.h
│   ├── sd-event.h
│   ├── sd-gpt.h
│   ├── sd-hwdb.h
│   ├── sd-id128.h
│   ├── sd-ipv4acd.h
│   ├── sd-ipv4ll.h
│   ├── sd-journal.h
│   ├── sd-json.h
│   ├── sd-lldp-rx.h
│   ├── sd-lldp-tx.h
│   ├── sd-lldp.h
│   ├── sd-login.h
│   ├── sd-messages.h
│   ├── sd-ndisc-neighbor.h
│   ├── sd-ndisc-protocol.h
│   ├── sd-ndisc-redirect.h
│   ├── sd-ndisc-router-solicit.h
│   ├── sd-ndisc-router.h
│   ├── sd-ndisc.h
│   ├── sd-netlink.h
│   ├── sd-network.h
│   ├── sd-path.h
│   ├── sd-radv.h
│   ├── sd-resolve.h
│   ├── sd-utf8.h
│   ├── sd-varlink-idl.h
│   └── sd-varlink.h
├── sysupdate
│   ├── meson.build
│   ├── org.freedesktop.sysupdate1.conf
│   ├── org.freedesktop.sysupdate1.policy
│   ├── org.freedesktop.sysupdate1.service
│   ├── sysupdate-cache.c
│   ├── sysupdate-cache.h
│   ├── sysupdate-feature.c
│   ├── sysupdate-feature.h
│   ├── sysupdate-forward.h
│   ├── sysupdate-instance.c
│   ├── sysupdate-instance.h
│   ├── sysupdate-partition.c
│   ├── sysupdate-partition.h
│   ├── sysupdate-pattern.c
│   ├── sysupdate-pattern.h
│   ├── sysupdate-resource.c
│   ├── sysupdate-resource.h
│   ├── sysupdate-transfer.c
│   ├── sysupdate-transfer.h
│   ├── sysupdate-update-set-flags.c
│   ├── sysupdate-update-set-flags.h
│   ├── sysupdate-update-set.c
│   ├── sysupdate-update-set.h
│   ├── sysupdate-util.c
│   ├── sysupdate-util.h
│   ├── sysupdate.c
│   ├── sysupdate.h
│   ├── sysupdated.c
│   └── updatectl.c
├── sysusers
│   ├── meson.build
│   └── sysusers.c
├── sysv-generator
│   ├── meson.build
│   └── sysv-generator.c
├── test
│   ├── generate-sym-test.py
│   ├── meson.build
│   ├── nss-test-util.c
│   ├── nss-test-util.h
│   ├── test-acl-util.c
│   ├── test-af-list.c
│   ├── test-alloc-util.c
│   ├── test-architecture.c
│   ├── test-argv-util.c
│   ├── test-arphrd-util.c
│   ├── test-ask-password-api.c
│   ├── test-async.c
│   ├── test-audit-util.c
│   ├── test-barrier.c
│   ├── test-binfmt-util.c
│   ├── test-bitfield.c
│   ├── test-bitmap.c
│   ├── test-blockdev-util.c
│   ├── test-boot-timestamps.c
│   ├── test-bootspec.c
│   ├── test-bpf-devices.c
│   ├── test-bpf-firewall.c
│   ├── test-bpf-foreign-programs.c
│   ├── test-bpf-restrict-fs.c
│   ├── test-bpf-token.c
│   ├── test-btrfs-physical-offset.c
│   ├── test-btrfs.c
│   ├── test-build-path.c
│   ├── test-bus-unit-util.c
│   ├── test-bus-util.c
│   ├── test-calendarspec.c
│   ├── test-capability-list.c
│   ├── test-capability-util.c
│   ├── test-cgroup-cpu.c
│   ├── test-cgroup-mask.c
│   ├── test-cgroup-unit-default.c
│   ├── test-cgroup-util.c
│   ├── test-cgroup.c
│   ├── test-chase-manual.c
│   ├── test-chase.c
│   ├── test-chid.c
│   ├── test-chown-rec.c
│   ├── test-clock.c
│   ├── test-color-util.c
│   ├── test-compare-operator.c
│   ├── test-compress-benchmark.c
│   ├── test-compress.c
│   ├── test-condition.c
│   ├── test-conf-files.c
│   ├── test-conf-parser.c
│   ├── test-copy.c
│   ├── test-core-unit.c
│   ├── test-coredump-util.c
│   ├── test-cpu-set-util.c
│   ├── test-creds.c
│   ├── test-cryptolib.c
│   ├── test-daemon.c
│   ├── test-data-fd-util.c
│   ├── test-date.c
│   ├── test-dev-setup.c
│   ├── test-device-nodes.c
│   ├── test-devnum-util.c
│   ├── test-dirent-util.c
│   ├── test-display-quota.c
│   ├── test-dlopen-so.c
│   ├── test-dlopen.c
│   ├── test-dns-domain.c
│   ├── test-ellipsize.c
│   ├── test-emergency-action.c
│   ├── test-engine.c
│   ├── test-env-file.c
│   ├── test-env-util.c
│   ├── test-errno-list.c
│   ├── test-errno-util.c
│   ├── test-escape.c
│   ├── test-ether-addr-util.c
│   ├── test-exec-util.c
│   ├── test-execute.c
│   ├── test-execve.c
│   ├── test-exit-status.c
│   ├── test-extract-word.c
│   ├── test-fd-util.c
│   ├── test-fdset.c
│   ├── test-fiemap.c
│   ├── test-fileio.c
│   ├── test-firewall-util.c
│   ├── test-format-table.c
│   ├── test-format-util.c
│   ├── test-fs-util.c
│   ├── test-fstab-util.c
│   ├── test-glob-util.c
│   ├── test-gpt.c
│   ├── test-gunicode.c
│   ├── test-hash-funcs.c
│   ├── test-hashmap-ordered.awk
│   ├── test-hashmap-plain.c
│   ├── test-hashmap.c
│   ├── test-hexdecoct.c
│   ├── test-hmac.c
│   ├── test-hostname-setup.c
│   ├── test-hostname-util.c
│   ├── test-id128.c
│   ├── test-image-filter.c
│   ├── test-image-policy.c
│   ├── test-import-util.c
│   ├── test-in-addr-prefix-util.c
│   ├── test-in-addr-util.c
│   ├── test-install-file.c
│   ├── test-install-root.c
│   ├── test-install.c
│   ├── test-io-util.c
│   ├── test-iovec-util.c
│   ├── test-ip-protocol-list.c
│   ├── test-ipcrm.c
│   ├── test-job-type.c
│   ├── test-journal-importer.c
│   ├── test-json.c
│   ├── test-kbd-util.c
│   ├── test-label.c
│   ├── test-libcrypt-util.c
│   ├── test-libmount.c
│   ├── test-limits-util.c
│   ├── test-list.c
│   ├── test-load-fragment.c
│   ├── test-local-addresses.c
│   ├── test-locale-util.c
│   ├── test-lock-util.c
│   ├── test-log.c
│   ├── test-logarithm.c
│   ├── test-login-util.c
│   ├── test-loop-block.c
│   ├── test-loopback.c
│   ├── test-macro.c
│   ├── test-math-util.c
│   ├── test-memfd-util.c
│   ├── test-memory-util.c
│   ├── test-mempool.c
│   ├── test-mempress.c
│   ├── test-memstream-util.c
│   ├── test-mkdir.c
│   ├── test-modhex.c
│   ├── test-mount-util.c
│   ├── test-mountpoint-util.c
│   ├── test-namespace.c
│   ├── test-net-naming-scheme.c
│   ├── test-netlink-manual.c
│   ├── test-nft-set.c
│   ├── test-notify-recv.c
│   ├── test-ns.c
│   ├── test-nsresource.c
│   ├── test-nss-hosts.c
│   ├── test-nss-users.c
│   ├── test-nulstr-util.c
│   ├── test-open-file.c
│   ├── test-openssl.c
│   ├── test-ordered-set.c
│   ├── test-os-util.c
│   ├── test-osc-context.c
│   ├── test-parse-argument.c
│   ├── test-parse-helpers.c
│   ├── test-parse-util.c
│   ├── test-path-lookup.c
│   ├── test-path-util.c
│   ├── test-path.c
│   ├── test-percent-util.c
│   ├── test-pidref.c
│   ├── test-pretty-print.c
│   ├── test-prioq.c
│   ├── test-proc-cmdline.c
│   ├── test-process-util.c
│   ├── test-procfs-util.c
│   ├── test-progress-bar.c
│   ├── test-psi-util.c
│   ├── test-qrcode-util.c
│   ├── test-random-util.c
│   ├── test-ratelimit.c
│   ├── test-raw-clone.c
│   ├── test-recovery-key.c
│   ├── test-recurse-dir.c
│   ├── test-replace-var.c
│   ├── test-rlimit-util.c
│   ├── test-rm-rf.c
│   ├── test-sbat.c
│   ├── test-sched-prio.c
│   ├── test-sd-hwdb.c
│   ├── test-sd-path.c
│   ├── test-seccomp.c
│   ├── test-secure-bits.c
│   ├── test-selinux.c
│   ├── test-serialize.c
│   ├── test-set-disable-mempool.c
│   ├── test-set.c
│   ├── test-sha1.c
│   ├── test-sha256.c
│   ├── test-shift-uid.c
│   ├── test-sigbus.c
│   ├── test-signal-util.c
│   ├── test-siphash24.c
│   ├── test-sizeof.c
│   ├── test-sleep-config.c
│   ├── test-socket-bind.c
│   ├── test-socket-netlink.c
│   ├── test-socket-util.c
│   ├── test-specifier.c
│   ├── test-stat-util.c
│   ├── test-static-destruct.c
│   ├── test-strbuf.c
│   ├── test-string-util.c
│   ├── test-strip-tab-ansi.c
│   ├── test-strv.c
│   ├── test-strxcpyx.c
│   ├── test-sysctl-util.c
│   ├── test-tables.c
│   ├── test-taint.c
│   ├── test-terminal-util.c
│   ├── test-tests.c
│   ├── test-time-util.c
│   ├── test-tmpfile-util.c
│   ├── test-tpm2.c
│   ├── test-udev-util.c
│   ├── test-uid-classification.c
│   ├── test-uid-range.c
│   ├── test-umask-util.c
│   ├── test-unaligned.c
│   ├── test-unit-file.c
│   ├── test-unit-name.c
│   ├── test-unit-serialize.c
│   ├── test-user-record.c
│   ├── test-user-util.c
│   ├── test-utf8.c
│   ├── test-utmp.c
│   ├── test-varlink-idl.c
│   ├── test-varlink.c
│   ├── test-verbs.c
│   ├── test-vpick.c
│   ├── test-watch-pid.c
│   ├── test-watchdog.c
│   ├── test-web-util.c
│   ├── test-xattr-util.c
│   └── test-xml.c
├── timedate
│   ├── hwclock-util.c
│   ├── hwclock-util.h
│   ├── meson.build
│   ├── org.freedesktop.timedate1.conf
│   ├── org.freedesktop.timedate1.policy
│   ├── org.freedesktop.timedate1.service
│   ├── timedatectl.c
│   └── timedated.c
├── timesync
│   ├── 80-systemd-timesync.list
│   ├── meson.build
│   ├── org.freedesktop.timesync1.conf
│   ├── org.freedesktop.timesync1.policy
│   ├── org.freedesktop.timesync1.service
│   ├── test-timesync.c
│   ├── timesyncd-bus.c
│   ├── timesyncd-bus.h
│   ├── timesyncd-conf.c
│   ├── timesyncd-conf.h
│   ├── timesyncd-forward.h
│   ├── timesyncd-gperf.gperf
│   ├── timesyncd-manager.c
│   ├── timesyncd-manager.h
│   ├── timesyncd-ntp-message.h
│   ├── timesyncd-server.c
│   ├── timesyncd-server.h
│   ├── timesyncd.c
│   ├── timesyncd.conf.in
│   └── wait-sync.c
├── tmpfiles
│   ├── meson.build
│   ├── offline-passwd.c
│   ├── offline-passwd.h
│   ├── test-offline-passwd.c
│   └── tmpfiles.c
├── tpm2-setup
│   ├── meson.build
│   ├── tpm2-clear.c
│   ├── tpm2-generator.c
│   └── tpm2-setup.c
├── tty-ask-password-agent
│   ├── meson.build
│   └── tty-ask-password-agent.c
├── udev
│   ├── ata_id
│   │   └── ata_id.c
│   ├── cdrom_id
│   │   └── cdrom_id.c
│   ├── dmi_memory_id
│   │   └── dmi_memory_id.c
│   ├── fido_id
│   │   ├── fido_id_desc.c
│   │   ├── fido_id_desc.h
│   │   ├── fido_id.c
│   │   ├── fuzz-fido-id-desc.c
│   │   └── test-fido-id-desc.c
│   ├── fuzz-udev-rule-parse-value.c
│   ├── fuzz-udev-rules.c
│   ├── fuzz-udev-rules.options
│   ├── generate-keyboard-keys-gperf.sh
│   ├── generate-keyboard-keys-list.sh
│   ├── iocost
│   │   ├── iocost.c
│   │   └── iocost.conf
│   ├── meson.build
│   ├── mtd_probe
│   │   ├── mtd_probe.c
│   │   ├── mtd_probe.h
│   │   └── probe_smartmedia.c
│   ├── net
│   │   ├── fuzz-link-parser.c
│   │   ├── fuzz-link-parser.options
│   │   ├── link-config-gperf.gperf
│   │   ├── link-config.c
│   │   ├── link-config.h
│   │   └── test-link-config-tables.c
│   ├── NOTES.md
│   ├── scsi_id
│   │   ├── README
│   │   ├── scsi_id.c
│   │   ├── scsi_id.h
│   │   ├── scsi_serial.c
│   │   └── scsi.h
│   ├── test-udev-builtin.c
│   ├── test-udev-format.c
│   ├── test-udev-manager.c
│   ├── test-udev-node.c
│   ├── test-udev-rule-runner.c
│   ├── test-udev-rules.c
│   ├── test-udev-spawn.c
│   ├── udev-builtin-blkid.c
│   ├── udev-builtin-btrfs.c
│   ├── udev-builtin-dissect_image.c
│   ├── udev-builtin-factory_reset.c
│   ├── udev-builtin-hwdb.c
│   ├── udev-builtin-input_id.c
│   ├── udev-builtin-keyboard.c
│   ├── udev-builtin-kmod.c
│   ├── udev-builtin-net_driver.c
│   ├── udev-builtin-net_id.c
│   ├── udev-builtin-net_setup_link.c
│   ├── udev-builtin-path_id.c
│   ├── udev-builtin-uaccess.c
│   ├── udev-builtin-usb_id.c
│   ├── udev-builtin.c
│   ├── udev-builtin.h
│   ├── udev-config.c
│   ├── udev-config.h
│   ├── udev-ctrl.c
│   ├── udev-ctrl.h
│   ├── udev-def.h
│   ├── udev-dump.c
│   ├── udev-dump.h
│   ├── udev-error.c
│   ├── udev-error.h
│   ├── udev-event.c
│   ├── udev-event.h
│   ├── udev-format.c
│   ├── udev-format.h
│   ├── udev-forward.h
│   ├── udev-manager-ctrl.c
│   ├── udev-manager-ctrl.h
│   ├── udev-manager.c
│   ├── udev-manager.h
│   ├── udev-node.c
│   ├── udev-node.h
│   ├── udev-rules.c
│   ├── udev-rules.h
│   ├── udev-spawn.c
│   ├── udev-spawn.h
│   ├── udev-trace.h
│   ├── udev-varlink.c
│   ├── udev-varlink.h
│   ├── udev-watch.c
│   ├── udev-watch.h
│   ├── udev-worker.c
│   ├── udev-worker.h
│   ├── udev.conf
│   ├── udev.pc.in
│   ├── udevadm-cat.c
│   ├── udevadm-control.c
│   ├── udevadm-hwdb.c
│   ├── udevadm-info.c
│   ├── udevadm-lock.c
│   ├── udevadm-monitor.c
│   ├── udevadm-settle.c
│   ├── udevadm-test-builtin.c
│   ├── udevadm-test.c
│   ├── udevadm-trigger.c
│   ├── udevadm-util.c
│   ├── udevadm-util.h
│   ├── udevadm-verify.c
│   ├── udevadm-wait.c
│   ├── udevadm.c
│   ├── udevadm.h
│   ├── udevd.c
│   ├── udevd.h
│   └── v4l_id
│       └── v4l_id.c
├── ukify
│   ├── test
│   │   ├── example.signing.crt.base64
│   │   ├── example.signing.key.base64
│   │   ├── example.tpm2-pcr-private.pem.base64
│   │   ├── example.tpm2-pcr-private2.pem.base64
│   │   ├── example.tpm2-pcr-public.pem.base64
│   │   ├── example.tpm2-pcr-public2.pem.base64
│   │   ├── meson.build
│   │   ├── pytest.ini
│   │   └── test_ukify.py
│   └── ukify.py
├── update-done
│   ├── meson.build
│   └── update-done.c
├── update-utmp
│   ├── meson.build
│   └── update-utmp.c
├── user-sessions
│   ├── meson.build
│   └── user-sessions.c
├── userdb
│   ├── 20-systemd-userdb.conf.in
│   ├── meson.build
│   ├── userdbctl.c
│   ├── userdbd-manager.c
│   ├── userdbd-manager.h
│   ├── userdbd.c
│   └── userwork.c
├── validatefs
│   ├── meson.build
│   └── validatefs.c
├── varlinkctl
│   ├── meson.build
│   └── varlinkctl.c
├── vconsole
│   ├── meson.build
│   └── vconsole-setup.c
├── veritysetup
│   ├── meson.build
│   ├── veritysetup-generator.c
│   └── veritysetup.c
├── version
│   ├── meson.build
│   └── version.h.in
├── vmspawn
│   ├── meson.build
│   ├── test-vmspawn-util.c
│   ├── vmspawn-mount.c
│   ├── vmspawn-mount.h
│   ├── vmspawn-register.c
│   ├── vmspawn-register.h
│   ├── vmspawn-scope.c
│   ├── vmspawn-scope.h
│   ├── vmspawn-settings.c
│   ├── vmspawn-settings.h
│   ├── vmspawn-util.c
│   ├── vmspawn-util.h
│   └── vmspawn.c
├── volatile-root
│   ├── meson.build
│   └── volatile-root.c
├── vpick
│   ├── meson.build
│   └── vpick-tool.c
└── xdg-autostart-generator
    ├── fuzz-xdg-desktop.c
    ├── fuzz-xdg-desktop.options
    ├── meson.build
    ├── test-xdg-autostart.c
    ├── xdg-autostart-condition.c
    ├── xdg-autostart-generator.c
    ├── xdg-autostart-service.c
    └── xdg-autostart-service.h

188 directories, 3219 files
