.
├── catalog
│   ├── meson.build
│   ├── systemd.be.catalog.in
│   ├── systemd.be@latin.catalog.in
│   ├── systemd.bg.catalog.in
│   ├── systemd.catalog.in
│   ├── systemd.da.catalog.in
│   ├── systemd.de.catalog.in
│   ├── systemd.fr.catalog.in
│   ├── systemd.hr.catalog.in
│   ├── systemd.hu.catalog.in
│   ├── systemd.it.catalog.in
│   ├── systemd.ko.catalog.in
│   ├── systemd.pl.catalog.in
│   ├── systemd.pt_BR.catalog.in
│   ├── systemd.ru.catalog.in
│   ├── systemd.sr.catalog.in
│   ├── systemd.zh_CN.catalog.in
│   └── systemd.zh_TW.catalog.in
├── CITATION.cff
├── coccinelle
│   ├── bool-cast.cocci
│   ├── bus-message-send.cocci
│   ├── close-above-stdio.cocci
│   ├── cmp.cocci
│   ├── cond-omit-middle.cocci
│   ├── const-strlen.disabled
│   ├── debug-logging.cocci
│   ├── div-round-up.cocci
│   ├── dup-fcntl.cocci
│   ├── empty-or-dash.cocci
│   ├── empty-or-root.cocci
│   ├── empty-to-null.cocci
│   ├── empty-to-root.cocci
│   ├── enotsup.cocci
│   ├── equals-null.cocci
│   ├── errno-check.cocci
│   ├── errno-wrapper.cocci
│   ├── errno.cocci
│   ├── exit-0.cocci
│   ├── flags-set.cocci
│   ├── fopen-unlocked.cocci
│   ├── free_and_replace.cocci
│   ├── hashmap_free.cocci
│   ├── htonl.cocci
│   ├── in_set.cocci
│   ├── iovec-make.cocci
│   ├── isempty.cocci
│   ├── log-json.cocci
│   ├── malloc_multiply.cocci
│   ├── mempcpy.cocci
│   ├── memzero.cocci
│   ├── mfree.cocci
│   ├── no-if-assignments.cocci
│   ├── not_in_set.cocci
│   ├── o-ndelay.cocci
│   ├── parsing_hacks.h
│   ├── reallocarray.cocci
│   ├── redundant-if.cocci
│   ├── run-coccinelle.sh
│   ├── safe_close-no-if.cocci
│   ├── safe_close.cocci
│   ├── safe_closedir.cocci
│   ├── safe_fclose.cocci
│   ├── sd_event_source_disable_unref.cocci
│   ├── set_ensure_put.cocci
│   ├── siphash24.cocci
│   ├── strdupa.cocci
│   ├── strempty.cocci
│   ├── strjoin.cocci
│   ├── strjoina.cocci
│   ├── strv_free.cocci
│   ├── swap-two.cocci
│   ├── synthetic-errno.cocci
│   ├── take-fd.cocci
│   ├── take-ptr.cocci
│   ├── timestamp-is-set.cocci
│   ├── while-true.cocci
│   ├── xsprintf.cocci
│   └── zz-drop-braces.cocci
├── docs
│   ├── _config.yml
│   ├── _data
│   │   └── extra_pages.json
│   ├── _includes
│   │   ├── footer.html
│   │   ├── head.html
│   │   └── header.html
│   ├── _layouts
│   │   ├── default.html
│   │   └── forward.html
│   ├── API_FILE_SYSTEMS.md
│   ├── APPSTREAM_BUNDLE.md
│   ├── ARCHITECTURE.md
│   ├── assets
│   │   ├── f17boot.png
│   │   ├── systemd-boot-menu.png
│   │   └── systemd-logo.svg
│   ├── AUTOMATIC_BOOT_ASSESSMENT.md
│   ├── BACKPORTS.md
│   ├── BLOCK_DEVICE_LOCKING.md
│   ├── BOOT_LOADER_INTERFACE.md
│   ├── BOOT_LOADER_SPECIFICATION.md
│   ├── BOOT.md
│   ├── BUILDING_IMAGES.md
│   ├── CATALOG.md
│   ├── CGROUP_DELEGATION.md
│   ├── CODE_OF_CONDUCT.md
│   ├── CODE_QUALITY.md
│   ├── CODING_STYLE.md
│   ├── CONTAINER_INTERFACE.md
│   ├── CONTRIBUTING.md
│   ├── CONTROL_GROUP_INTERFACE.md
│   ├── CONVERTING_TO_HOMED.md
│   ├── COREDUMP_PACKAGE_METADATA.md
│   ├── COREDUMP.md
│   ├── CREDENTIALS.md
│   ├── DAEMON_SOCKET_ACTIVATION.md
│   ├── DEBUGGING.md
│   ├── DESKTOP_ENVIRONMENTS.md
│   ├── DISCOVERABLE_PARTITIONS.md
│   ├── DISK-QUOTAS-PROJECTIDS.md
│   ├── DISTRO_PORTING.md
│   ├── ELF_DLOPEN_METADATA.md
│   ├── ELF_PACKAGE_METADATA.md
│   ├── ENVIRONMENT.md
│   ├── FACTORY_RESET.md
│   ├── FAQ.md
│   ├── favicon.png
│   ├── favicon.svg
│   ├── FILE_DESCRIPTOR_STORE.md
│   ├── fonts
│   │   ├── heebo-bold.woff
│   │   └── heebo-regular.woff
│   ├── GROUP_RECORD.md
│   ├── HACKING.md
│   ├── HOME_DIRECTORY.md
│   ├── INCOMPATIBILITIES.md
│   ├── index.md
│   ├── INHIBITOR_LOCKS.md
│   ├── INITRD_INTERFACE.md
│   ├── JOURNAL_EXPORT_FORMATS.md
│   ├── JOURNAL_FILE_FORMAT.md
│   ├── JOURNAL_NATIVE_PROTOCOL.md
│   ├── MEMORY_PRESSURE.md
│   ├── MINIMAL_BUILDS.md
│   ├── MOUNT_REQUIREMENTS.md
│   ├── MY_SERVICE_CANT_GET_REALTIME.md
│   ├── NETWORK_ONLINE.md
│   ├── OPTIMIZATIONS.md
│   ├── OSC-CONTEXT.md
│   ├── PACKAGE_METADATA_FOR_EXECUTABLE_FILES.md
│   ├── PASSWORD_AGENTS.md
│   ├── PAX_CONTROL_GROUPS.md
│   ├── PORTABILITY_AND_STABILITY.md
│   ├── PORTABLE_SERVICES.md
│   ├── PORTING_TO_NEW_ARCHITECTURES.md
│   ├── PREDICTABLE_INTERFACE_NAMES.md
│   ├── PRESET.md
│   ├── RANDOM_SEEDS.md
│   ├── RELEASE.md
│   ├── RESOLVED-VPNS.md
│   ├── ROOT_STORAGE_DAEMONS.md
│   ├── ROOTFS_DISCOVERY.md
│   ├── rootfs-discovery-flow.svg
│   ├── SECURITY.md
│   ├── SEPARATE_USR_IS_BROKEN.md
│   ├── style.css
│   ├── SYSLOG.md
│   ├── SYSTEMD_FILE_HIERARCHY_REQUIREMENTS.md
│   ├── sysvinit
│   │   ├── meson.build
│   │   └── README.in
│   ├── TEMPORARY_DIRECTORIES.md
│   ├── TESTING_WITH_SANITIZERS.md
│   ├── THE_CASE_FOR_THE_USR_MERGE.md
│   ├── TIPS_AND_TRICKS.md
│   ├── TPM2_PCR_MEASUREMENTS.md
│   ├── TRANSIENT-SETTINGS.md
│   ├── TRANSLATORS.md
│   ├── UIDS-GIDS.md
│   ├── USER_GROUP_API.md
│   ├── USER_NAMES.md
│   ├── USER_RECORD_BLOB_DIRS.md
│   ├── USER_RECORD.md
│   ├── USERDB_AND_DESKTOPS.md
│   ├── var-log
│   │   ├── meson.build
│   │   └── README.logs
│   ├── VM_INTERFACE.md
│   ├── WRITING_DESKTOP_ENVIRONMENTS.md
│   ├── WRITING_DISPLAY_MANAGERS.md
│   ├── WRITING_NETWORK_CONFIGURATION_MANAGERS.md
│   ├── WRITING_RESOLVER_CLIENTS.md
│   └── WRITING_VM_AND_CONTAINER_MANAGERS.md
├── factory
│   ├── etc
│   │   ├── issue
│   │   ├── nsswitch.conf
│   │   └── pam.d
│   │       ├── other
│   │       └── system-auth
│   └── templates
│       ├── locale.conf.in
│       ├── meson.build
│       └── vconsole.conf.in
├── hwdb.d
│   ├── 20-acpi-vendor.hwdb
│   ├── 20-acpi-vendor.hwdb.patch
│   ├── 20-bluetooth-vendor-product.hwdb
│   ├── 20-dmi-id.hwdb
│   ├── 20-net-ifname.hwdb
│   ├── 20-OUI.hwdb
│   ├── 20-pci-classes.hwdb
│   ├── 20-pci-vendor-model.hwdb
│   ├── 20-sdio-classes.hwdb
│   ├── 20-sdio-vendor-model.hwdb
│   ├── 20-usb-classes.hwdb
│   ├── 20-usb-vendor-model.hwdb
│   ├── 20-vmbus-class.hwdb
│   ├── 60-autosuspend-fingerprint-reader.hwdb
│   ├── 60-autosuspend.hwdb
│   ├── 60-evdev.hwdb
│   ├── 60-input-id.hwdb
│   ├── 60-keyboard.hwdb
│   ├── 60-seat.hwdb
│   ├── 60-sensor.hwdb
│   ├── 70-analyzers.hwdb
│   ├── 70-av-production.hwdb
│   ├── 70-cameras.hwdb
│   ├── 70-hardware-wallets.hwdb
│   ├── 70-joystick.hwdb
│   ├── 70-lights.hwdb
│   ├── 70-maker-tools.hwdb
│   ├── 70-mouse.hwdb
│   ├── 70-pda.hwdb
│   ├── 70-pointingstick.hwdb
│   ├── 70-software-radio.hwdb
│   ├── 70-sound-card.hwdb
│   ├── 70-touchpad.hwdb
│   ├── 80-ieee1394-unit-function.hwdb
│   ├── 82-net-auto-link-local.hwdb
│   ├── acpi_id_registry.csv
│   ├── acpi-update.py
│   ├── ids_parser.py
│   ├── ma-large.txt
│   ├── ma-medium.txt
│   ├── ma-small.txt
│   ├── meson.build
│   ├── parse_hwdb.py
│   ├── pci.ids
│   ├── pnp_id_registry.csv
│   ├── README
│   ├── sdio.ids
│   └── usb.ids
├── LICENSE.GPL2
├── LICENSE.LGPL2.1
├── LICENSES
│   ├── alg-sha1-public-domain.txt
│   ├── BSD-2-Clause.txt
│   ├── BSD-3-Clause.txt
│   ├── CC0-1.0.txt
│   ├── LGPL-2.0-or-later.txt
│   ├── Linux-syscall-note.txt
│   ├── lookup3-public-domain.txt
│   ├── MIT-0.txt
│   ├── MIT.txt
│   ├── murmurhash2-public-domain.txt
│   ├── OFL-1.1.txt
│   └── README.md
├── man
│   ├── 50-xdg-data-dirs.sh
│   ├── 90-rearrange-path.py
│   ├── binfmt.d.xml
│   ├── bootctl.xml
│   ├── bootup.xml
│   ├── busctl.xml
│   ├── capsule@.service.xml
│   ├── cgroup-sandboxing.xml
│   ├── check-os-release-simple.py
│   ├── check-os-release.py
│   ├── check-os-release.sh
│   ├── common-variables.xml
│   ├── coredump.conf.xml
│   ├── coredumpctl.xml
│   ├── crypttab.xml
│   ├── custom-entities.ent.in
│   ├── custom-html.xsl
│   ├── custom-man.xsl
│   ├── daemon.xml
│   ├── directives-template.xml
│   ├── dnssec-trust-anchors.d.xml
│   ├── environment.d.xml
│   ├── event-quick-child.c
│   ├── fido2-crypttab.sh
│   ├── file-hierarchy.xml
│   ├── glib-event-glue.c
│   ├── homectl.xml
│   ├── homed.conf.xml
│   ├── hostname.xml
│   ├── hostnamectl.xml
│   ├── html.in
│   ├── hwdb-usb-device.c
│   ├── hwdb.xml
│   ├── id128-app-specific.c
│   ├── importctl.xml
│   ├── inotify-watch-tmp.c
│   ├── integritytab.xml
│   ├── iocost.conf.xml
│   ├── journal-enumerate-fields.c
│   ├── journal-iterate-foreach.c
│   ├── journal-iterate-poll.c
│   ├── journal-iterate-unique.c
│   ├── journal-iterate-wait.c
│   ├── journal-remote.conf.xml
│   ├── journal-stream-fd.c
│   ├── journal-upload.conf.xml
│   ├── journalctl.xml
│   ├── journald.conf.xml
│   ├── kernel-command-line.xml
│   ├── kernel-install.xml
│   ├── libsystemd-pkgconfig.xml
│   ├── libsystemd.xml
│   ├── libudev.xml
│   ├── loader.conf.xml
│   ├── locale.conf.xml
│   ├── localectl.xml
│   ├── localtime.xml
│   ├── logcontrol-example.c
│   ├── loginctl.xml
│   ├── logind.conf.xml
│   ├── machine-id.xml
│   ├── machine-info.xml
│   ├── machinectl.xml
│   ├── man.in
│   ├── meson.build
│   ├── modules-load.d.xml
│   ├── networkctl.xml
│   ├── networkd.conf.xml
│   ├── notify-selfcontained-example.c
│   ├── notify-selfcontained-example.py
│   ├── nss-myhostname.xml
│   ├── nss-mymachines.xml
│   ├── nss-resolve.xml
│   ├── nss-systemd.xml
│   ├── oomctl.xml
│   ├── oomd.conf.xml
│   ├── org.freedesktop.home1.xml
│   ├── org.freedesktop.hostname1.xml
│   ├── org.freedesktop.import1.xml
│   ├── org.freedesktop.locale1.xml
│   ├── org.freedesktop.LogControl1.xml
│   ├── org.freedesktop.login1.xml
│   ├── org.freedesktop.machine1.xml
│   ├── org.freedesktop.network1.xml
│   ├── org.freedesktop.oom1.xml
│   ├── org.freedesktop.portable1.xml
│   ├── org.freedesktop.resolve1.xml
│   ├── org.freedesktop.systemd1.xml
│   ├── org.freedesktop.sysupdate1.xml
│   ├── org.freedesktop.timedate1.xml
│   ├── org.freedesktop.timesync1.xml
│   ├── os-release.xml
│   ├── pam_systemd_home.xml
│   ├── pam_systemd_loadkey.xml
│   ├── pam_systemd.xml
│   ├── path-documents.c
│   ├── portablectl.xml
│   ├── poweroff.xml
│   ├── print-unit-path-call-method.c
│   ├── print-unit-path.c
│   ├── pstore.conf.xml
│   ├── repart.d.xml
│   ├── resolvectl.xml
│   ├── resolved.conf.xml
│   ├── rules
│   │   └── meson.build
│   ├── run0.xml
│   ├── sd_booted.xml
│   ├── sd_bus_add_match.xml
│   ├── sd_bus_add_node_enumerator.xml
│   ├── sd_bus_add_object_manager.xml
│   ├── sd_bus_add_object.xml
│   ├── sd_bus_attach_event.xml
│   ├── sd_bus_call_method.xml
│   ├── sd_bus_call.xml
│   ├── sd_bus_can_send.xml
│   ├── sd_bus_close.xml
│   ├── sd_bus_creds_get_pid.xml
│   ├── sd_bus_creds_new_from_pid.xml
│   ├── sd_bus_default.xml
│   ├── sd_bus_emit_signal.xml
│   ├── sd_bus_enqueue_for_read.xml
│   ├── sd_bus_error_add_map.xml
│   ├── sd_bus_error-example.c
│   ├── sd_bus_error.xml
│   ├── sd_bus_get_current_handler.xml
│   ├── sd_bus_get_fd.xml
│   ├── sd_bus_get_n_queued_read.xml
│   ├── sd_bus_get_name_creds.xml
│   ├── sd_bus_get_name_machine_id.xml
│   ├── sd_bus_interface_name_is_valid.xml
│   ├── sd_bus_is_open.xml
│   ├── sd_bus_list_names.xml
│   ├── sd_bus_message_append_array.xml
│   ├── sd_bus_message_append_basic.xml
│   ├── sd_bus_message_append_string_memfd.xml
│   ├── sd_bus_message_append_strv.xml
│   ├── sd_bus_message_append.xml
│   ├── sd_bus_message_at_end.xml
│   ├── sd_bus_message_copy.xml
│   ├── sd_bus_message_dump.xml
│   ├── sd_bus_message_get_cookie.xml
│   ├── sd_bus_message_get_monotonic_usec.xml
│   ├── sd_bus_message_get_signature.xml
│   ├── sd_bus_message_get_type.xml
│   ├── sd_bus_message_new_method_call.xml
│   ├── sd_bus_message_new_method_error.xml
│   ├── sd_bus_message_new_signal.xml
│   ├── sd_bus_message_new.xml
│   ├── sd_bus_message_open_container.xml
│   ├── sd_bus_message_read_array.xml
│   ├── sd_bus_message_read_basic.xml
│   ├── sd_bus_message_read_strv.xml
│   ├── sd_bus_message_read.xml
│   ├── sd_bus_message_rewind.xml
│   ├── sd_bus_message_seal.xml
│   ├── sd_bus_message_sensitive.xml
│   ├── sd_bus_message_set_destination.xml
│   ├── sd_bus_message_set_expect_reply.xml
│   ├── sd_bus_message_skip.xml
│   ├── sd_bus_message_verify_type.xml
│   ├── sd_bus_negotiate_fds.xml
│   ├── sd_bus_new.xml
│   ├── sd_bus_path_encode.xml
│   ├── sd_bus_pending_method_calls.xml
│   ├── sd_bus_process.xml
│   ├── sd_bus_query_sender_creds.xml
│   ├── sd_bus_reply_method_error.xml
│   ├── sd_bus_reply_method_return.xml
│   ├── sd_bus_request_name.xml
│   ├── sd_bus_send.xml
│   ├── sd_bus_service_reconnect.c
│   ├── sd_bus_set_address.xml
│   ├── sd_bus_set_close_on_exit.xml
│   ├── sd_bus_set_connected_signal.xml
│   ├── sd_bus_set_description.xml
│   ├── sd_bus_set_exit_on_disconnect.xml
│   ├── sd_bus_set_fd.xml
│   ├── sd_bus_set_method_call_timeout.xml
│   ├── sd_bus_set_property.xml
│   ├── sd_bus_set_sender.xml
│   ├── sd_bus_set_server.xml
│   ├── sd_bus_set_watch_bind.xml
│   ├── sd_bus_slot_get_bus.xml
│   ├── sd_bus_slot_ref.xml
│   ├── sd_bus_slot_set_description.xml
│   ├── sd_bus_slot_set_destroy_callback.xml
│   ├── sd_bus_slot_set_floating.xml
│   ├── sd_bus_slot_set_userdata.xml
│   ├── sd_bus_start.xml
│   ├── sd_bus_track_add_name.xml
│   ├── sd_bus_track_new.xml
│   ├── sd_bus_wait.xml
│   ├── sd_device_enumerator_add_match_parent-example.c
│   ├── sd_device_enumerator_add_match_parent.xml
│   ├── sd_device_enumerator_get_device_first.xml
│   ├── sd_device_enumerator_new-example.c
│   ├── sd_device_enumerator_new.xml
│   ├── sd_device_get_syspath.xml
│   ├── sd_device_ref.xml
│   ├── sd_event_add_child.xml
│   ├── sd_event_add_defer.xml
│   ├── sd_event_add_inotify.xml
│   ├── sd_event_add_io.xml
│   ├── sd_event_add_memory_pressure.xml
│   ├── sd_event_add_signal.xml
│   ├── sd_event_add_time.xml
│   ├── sd_event_exit.xml
│   ├── sd_event_get_fd.xml
│   ├── sd_event_new.xml
│   ├── sd_event_now.xml
│   ├── sd_event_run.xml
│   ├── sd_event_set_signal_exit.xml
│   ├── sd_event_set_watchdog.xml
│   ├── sd_event_source_get_event.xml
│   ├── sd_event_source_get_pending.xml
│   ├── sd_event_source_set_description.xml
│   ├── sd_event_source_set_destroy_callback.xml
│   ├── sd_event_source_set_enabled.xml
│   ├── sd_event_source_set_exit_on_failure.xml
│   ├── sd_event_source_set_floating.xml
│   ├── sd_event_source_set_prepare.xml
│   ├── sd_event_source_set_priority.xml
│   ├── sd_event_source_set_ratelimit.xml
│   ├── sd_event_source_set_userdata.xml
│   ├── sd_event_source_unref.xml
│   ├── sd_event_wait.xml
│   ├── sd_get_seats.xml
│   ├── sd_hwdb_get.xml
│   ├── sd_hwdb_new.xml
│   ├── sd_id128_get_machine.xml
│   ├── sd_id128_randomize.xml
│   ├── sd_id128_to_string.xml
│   ├── sd_is_fifo.xml
│   ├── sd_journal_add_match.xml
│   ├── sd_journal_enumerate_fields.xml
│   ├── sd_journal_get_catalog.xml
│   ├── sd_journal_get_cursor.xml
│   ├── sd_journal_get_cutoff_realtime_usec.xml
│   ├── sd_journal_get_data.xml
│   ├── sd_journal_get_fd.xml
│   ├── sd_journal_get_realtime_usec.xml
│   ├── sd_journal_get_seqnum.xml
│   ├── sd_journal_get_usage.xml
│   ├── sd_journal_has_runtime_files.xml
│   ├── sd_journal_next.xml
│   ├── sd_journal_open.xml
│   ├── sd_journal_print.xml
│   ├── sd_journal_query_unique.xml
│   ├── sd_journal_seek_head.xml
│   ├── sd_journal_stream_fd.xml
│   ├── sd_listen_fds.xml
│   ├── sd_login_monitor_new.xml
│   ├── sd_machine_get_class.xml
│   ├── sd_notify.xml
│   ├── sd_path_lookup.xml
│   ├── sd_pid_get_owner_uid.xml
│   ├── sd_pidfd_get_inode_id.xml
│   ├── sd_seat_get_active.xml
│   ├── sd_session_is_active.xml
│   ├── sd_uid_get_state.xml
│   ├── sd_varlink_push_fd.xml
│   ├── sd_varlink_send.xml
│   ├── sd_varlink_set_description.xml
│   ├── sd_watchdog_enabled.xml
│   ├── sd-bus-container-append.c
│   ├── sd-bus-container-read.c
│   ├── sd-bus-errors.xml
│   ├── sd-bus.xml
│   ├── sd-daemon.xml
│   ├── sd-device.xml
│   ├── sd-event.xml
│   ├── sd-hwdb.xml
│   ├── sd-id128.xml
│   ├── sd-journal.xml
│   ├── sd-json.xml
│   ├── sd-login.xml
│   ├── sd-varlink.xml
│   ├── send-unit-files-changed.c
│   ├── shutdown.xml
│   ├── smbios-type-11.xml
│   ├── standard-conf.xml
│   ├── standard-options.xml
│   ├── standard-specifiers.xml
│   ├── supported-controllers.xml
│   ├── sysctl.d.xml
│   ├── system-only.xml
│   ├── system-or-user-ns.xml
│   ├── systemctl.xml
│   ├── systemd-ac-power.xml
│   ├── systemd-analyze.xml
│   ├── systemd-ask-password-console.service.xml
│   ├── systemd-ask-password.xml
│   ├── systemd-backlight@.service.xml
│   ├── systemd-battery-check.service.xml
│   ├── systemd-binfmt.service.xml
│   ├── systemd-bless-boot-generator.xml
│   ├── systemd-bless-boot.service.xml
│   ├── systemd-boot-check-no-failures.service.xml
│   ├── systemd-boot-clear-sysfail.service.xml
│   ├── systemd-boot-random-seed.service.xml
│   ├── systemd-boot.xml
│   ├── systemd-bsod.service.xml
│   ├── systemd-cat.xml
│   ├── systemd-cgls.xml
│   ├── systemd-cgtop.xml
│   ├── systemd-coredump.xml
│   ├── systemd-creds.xml
│   ├── systemd-cryptenroll.xml
│   ├── systemd-cryptsetup-generator.xml
│   ├── systemd-cryptsetup.xml
│   ├── systemd-debug-generator.xml
│   ├── systemd-delta.xml
│   ├── systemd-detect-virt.xml
│   ├── systemd-dissect.xml
│   ├── systemd-environment-d-generator.xml
│   ├── systemd-escape.xml
│   ├── systemd-factory-reset-generator.xml
│   ├── systemd-factory-reset.xml
│   ├── systemd-firstboot.xml
│   ├── systemd-fsck@.service.xml
│   ├── systemd-fstab-generator.xml
│   ├── systemd-getty-generator.xml
│   ├── systemd-gpt-auto-generator.xml
│   ├── systemd-hibernate-resume-generator.xml
│   ├── systemd-hibernate-resume.service.xml
│   ├── systemd-homed.service.xml
│   ├── systemd-hostnamed.service.xml
│   ├── systemd-hwdb.xml
│   ├── systemd-id128.xml
│   ├── systemd-import-generator.xml
│   ├── systemd-importd.service.xml
│   ├── systemd-inhibit.xml
│   ├── systemd-integritysetup-generator.xml
│   ├── systemd-integritysetup@.service.xml
│   ├── systemd-journal-gatewayd.service.xml
│   ├── systemd-journal-remote.service.xml
│   ├── systemd-journal-upload.service.xml
│   ├── systemd-journald.service.xml
│   ├── systemd-keyutil.xml
│   ├── systemd-localed.service.xml
│   ├── systemd-logind.service.xml
│   ├── systemd-loop@.service.xml
│   ├── systemd-machine-id-commit.service.xml
│   ├── systemd-machine-id-setup.xml
│   ├── systemd-machined.service.xml
│   ├── systemd-makefs@.service.xml
│   ├── systemd-measure.xml
│   ├── systemd-modules-load.service.xml
│   ├── systemd-mount.xml
│   ├── systemd-mountfsd.service.xml
│   ├── systemd-network-generator.service.xml
│   ├── systemd-networkd-wait-online.service.xml
│   ├── systemd-networkd.service.xml
│   ├── systemd-notify.xml
│   ├── systemd-nspawn.xml
│   ├── systemd-nsresourced.service.xml
│   ├── systemd-oomd.service.xml
│   ├── systemd-path.xml
│   ├── systemd-pcrlock.xml
│   ├── systemd-pcrphase.service.xml
│   ├── systemd-portabled.service.xml
│   ├── systemd-poweroff.service.xml
│   ├── systemd-pstore.service.xml
│   ├── systemd-pty-forward.xml
│   ├── systemd-quotacheck.service.xml
│   ├── systemd-random-seed.service.xml
│   ├── systemd-rc-local-generator.xml
│   ├── systemd-remount-fs.service.xml
│   ├── systemd-repart.xml
│   ├── systemd-resolved.service.xml
│   ├── systemd-rfkill.service.xml
│   ├── systemd-run-generator.xml
│   ├── systemd-run.xml
│   ├── systemd-sbsign.xml
│   ├── systemd-sleep.conf.xml
│   ├── systemd-socket-activate.xml
│   ├── systemd-socket-proxyd.xml
│   ├── systemd-soft-reboot.service.xml
│   ├── systemd-ssh-generator.xml
│   ├── systemd-ssh-issue.xml
│   ├── systemd-ssh-proxy.xml
│   ├── systemd-stdio-bridge.xml
│   ├── systemd-storagetm.service.xml
│   ├── systemd-stub.xml
│   ├── systemd-suspend.service.xml
│   ├── systemd-sysctl.service.xml
│   ├── systemd-sysext.xml
│   ├── systemd-system-update-generator.xml
│   ├── systemd-system.conf.xml
│   ├── systemd-sysupdate.xml
│   ├── systemd-sysupdated.service.xml
│   ├── systemd-sysusers.xml
│   ├── systemd-sysv-generator.xml
│   ├── systemd-time-wait-sync.service.xml
│   ├── systemd-timedated.service.xml
│   ├── systemd-timesyncd.service.xml
│   ├── systemd-tmpfiles.xml
│   ├── systemd-tpm2-clear.service.xml
│   ├── systemd-tpm2-generator.xml
│   ├── systemd-tpm2-setup.service.xml
│   ├── systemd-tty-ask-password-agent.xml
│   ├── systemd-udev-settle.service.xml
│   ├── systemd-udevd.service.xml
│   ├── systemd-update-done.service.xml
│   ├── systemd-update-utmp.service.xml
│   ├── systemd-user-sessions.service.xml
│   ├── systemd-userdbd.service.xml
│   ├── systemd-validatefs@.service.xml
│   ├── systemd-vconsole-setup.service.xml
│   ├── systemd-veritysetup-generator.xml
│   ├── systemd-veritysetup@.service.xml
│   ├── systemd-vmspawn.xml
│   ├── systemd-volatile-root.service.xml
│   ├── systemd-vpick.xml
│   ├── systemd-xdg-autostart-generator.xml
│   ├── systemd.automount.xml
│   ├── systemd.device.xml
│   ├── systemd.dns-delegate.xml
│   ├── systemd.dnssd.xml
│   ├── systemd.environment-generator.xml
│   ├── systemd.exec.xml
│   ├── systemd.generator.xml
│   ├── systemd.image-filter.xml
│   ├── systemd.image-policy.xml
│   ├── systemd.journal-fields.xml
│   ├── systemd.kill.xml
│   ├── systemd.link.xml
│   ├── systemd.mount.xml
│   ├── systemd.net-naming-scheme.xml
│   ├── systemd.netdev.xml
│   ├── systemd.network.xml
│   ├── systemd.nspawn.xml
│   ├── systemd.offline-updates.xml
│   ├── systemd.path.xml
│   ├── systemd.pcrlock.xml
│   ├── systemd.preset.xml
│   ├── systemd.resource-control.xml
│   ├── systemd.scope.xml
│   ├── systemd.service.xml
│   ├── systemd.slice.xml
│   ├── systemd.socket.xml
│   ├── systemd.special.xml
│   ├── systemd.swap.xml
│   ├── systemd.syntax.xml
│   ├── systemd.system-credentials.xml
│   ├── systemd.target.xml
│   ├── systemd.time.xml
│   ├── systemd.timer.xml
│   ├── systemd.unit.xml
│   ├── systemd.v.xml
│   ├── systemd.xml
│   ├── sysupdate.d.xml
│   ├── sysupdate.features.xml
│   ├── sysusers.d.xml
│   ├── tc.xml
│   ├── threads-aware.xml
│   ├── timedatectl.xml
│   ├── timesyncd.conf.xml
│   ├── tmpfiles.d.xml
│   ├── tpm2-crypttab.sh
│   ├── udev_device_get_syspath.xml
│   ├── udev_device_has_tag.xml
│   ├── udev_device_new_from_syspath.xml
│   ├── udev_enumerate_add_match_subsystem.xml
│   ├── udev_enumerate_new.xml
│   ├── udev_enumerate_scan_devices.xml
│   ├── udev_list_entry.xml
│   ├── udev_monitor_filter_update.xml
│   ├── udev_monitor_new_from_netlink.xml
│   ├── udev_monitor_receive_device.xml
│   ├── udev_new.xml
│   ├── udev.conf.xml
│   ├── udev.xml
│   ├── udevadm.xml
│   ├── uki.conf.example
│   ├── ukify_hwid.json.example
│   ├── ukify.xml
│   ├── unit-states.xml
│   ├── updatectl.xml
│   ├── user-system-options.xml
│   ├── user@.service.xml
│   ├── userdbctl.xml
│   ├── varlinkctl.xml
│   ├── vconsole.conf.xml
│   ├── veritytab.xml
│   ├── version-info.xml
│   ├── vpick.xml
│   ├── vtable-example.c
│   ├── vtable-example.xml
│   └── yubikey-crypttab.sh
├── meson_options.txt
├── meson.build
├── meson.version
├── mime
│   ├── io.systemd.xml
│   └── meson.build
├── mkosi
│   ├── keydev.repart
│   │   └── 00-root.conf
│   ├── mkosi.clangd
│   ├── mkosi.clean
│   ├── mkosi.conf
│   ├── mkosi.conf.d
│   │   ├── arch
│   │   │   ├── mkosi.conf
│   │   │   ├── mkosi.conf.d
│   │   │   │   ├── debug.conf
│   │   │   │   └── pkgenv.conf
│   │   │   └── systemd.prepare
│   │   ├── build.conf
│   │   ├── centos
│   │   │   └── mkosi.conf
│   │   ├── centos-fedora
│   │   │   ├── mkosi.conf
│   │   │   ├── mkosi.conf.d
│   │   │   │   ├── debug.conf
│   │   │   │   ├── efi.conf
│   │   │   │   ├── pkgenv.conf
│   │   │   │   └── selinux.conf
│   │   │   ├── mkosi.prepare
│   │   │   └── systemd.prepare
│   │   ├── debian
│   │   │   ├── mkosi.conf
│   │   │   └── mkosi.conf.d
│   │   │       ├── arm64.conf
│   │   │       └── x86-64.conf
│   │   ├── debian-ubuntu
│   │   │   ├── mkosi.conf
│   │   │   ├── mkosi.conf.d
│   │   │   │   ├── debug.conf
│   │   │   │   ├── efi-debug.conf
│   │   │   │   ├── efi.conf
│   │   │   │   ├── network.conf
│   │   │   │   └── pkgenv.conf
│   │   │   └── systemd.prepare
│   │   ├── extra-search-path.conf
│   │   ├── fedora
│   │   │   ├── mkosi.conf
│   │   │   └── mkosi.conf.d
│   │   │       └── rawhide-42.conf
│   │   ├── none.conf
│   │   ├── opensuse
│   │   │   ├── macros.db_backend
│   │   │   ├── mkosi.conf
│   │   │   ├── mkosi.conf.d
│   │   │   │   ├── debug.conf
│   │   │   │   ├── efi-debug.conf
│   │   │   │   ├── efi.conf
│   │   │   │   └── pkgenv.conf
│   │   │   └── systemd.prepare
│   │   └── ubuntu
│   │       ├── mkosi.conf
│   │       ├── mkosi.conf.d
│   │       │   ├── non-x86.conf
│   │       │   └── x86.conf
│   │       ├── noble-backports-ports.sources
│   │       └── noble-backports.sources
│   ├── mkosi.coverage
│   │   ├── mkosi.conf
│   │   └── mkosi.postinst
│   ├── mkosi.credentials
│   │   ├── keyfile
│   │   ├── userdb.group.testuser
│   │   └── userdb.user.testuser
│   ├── mkosi.extra
│   │   ├── etc
│   │   │   └── iscsi
│   │   │       └── iscsid.conf
│   │   ├── root
│   │   └── usr
│   │       ├── lib
│   │       │   ├── sysctl.d
│   │       │   │   └── 99-apparmor-unpriv-userns.conf
│   │       │   ├── systemd
│   │       │   │   └── system
│   │       │   │       └── user@.service.d
│   │       │   │           └── 99-SYSTEMD_UNIT_PATH.conf
│   │       │   └── tmpfiles.d
│   │       │       └── snapshot.conf
│   │       └── share
│   │           └── dbus-1
│   │               └── system.d
│   │                   └── systemd.test.ExecStopPost.conf
│   ├── mkosi.extra.common
│   │   ├── etc
│   │   │   └── issue
│   │   └── usr
│   │       └── lib
│   │           └── systemd
│   │               ├── coredump.conf.d
│   │               │   └── 10-coredump-journal-storage.conf
│   │               ├── coverage-forwarder
│   │               ├── journald.conf.d
│   │               │   └── ratelimit.conf
│   │               ├── system
│   │               │   └── coverage-forwarder.service
│   │               └── system-preset
│   │                   ├── 00-mkosi.preset
│   │                   └── 99-mkosi.preset
│   ├── mkosi.finalize
│   ├── mkosi.functions
│   ├── mkosi.images
│   │   ├── build
│   │   │   ├── mkosi.conf
│   │   │   └── mkosi.conf.d
│   │   │       ├── arch
│   │   │       │   ├── mkosi.build.chroot
│   │   │       │   ├── mkosi.conf
│   │   │       │   └── mkosi.prepare
│   │   │       ├── centos
│   │   │       │   ├── mkosi.conf
│   │   │       │   └── mkosi.conf.d
│   │   │       │       ├── erofs-utils.conf
│   │   │       │       └── rpmautospec-rpm-macros.conf
│   │   │       ├── centos-fedora
│   │   │       │   ├── mkosi.build.chroot
│   │   │       │   ├── mkosi.conf
│   │   │       │   └── mkosi.prepare
│   │   │       ├── debian-ubuntu
│   │   │       │   ├── mkosi.build.chroot
│   │   │       │   ├── mkosi.conf
│   │   │       │   └── mkosi.prepare
│   │   │       ├── fedora
│   │   │       │   └── mkosi.conf
│   │   │       └── opensuse
│   │   │           ├── mkosi.build.chroot
│   │   │           ├── mkosi.conf
│   │   │           └── mkosi.prepare
│   │   ├── exitrd
│   │   │   ├── mkosi.conf
│   │   │   ├── mkosi.conf.d
│   │   │   │   ├── arch.conf
│   │   │   │   ├── build.conf
│   │   │   │   ├── centos-fedora.conf
│   │   │   │   ├── debian.conf
│   │   │   │   ├── opensuse.conf
│   │   │   │   └── ubuntu.conf
│   │   │   └── mkosi.extra
│   │   │       └── shutdown
│   │   ├── initrd
│   │   │   ├── mkosi.conf
│   │   │   ├── mkosi.conf.d
│   │   │   │   ├── arch.conf
│   │   │   │   ├── build.conf
│   │   │   │   ├── centos-fedora.conf
│   │   │   │   ├── debian-ubuntu.conf
│   │   │   │   ├── fedora.conf
│   │   │   │   └── opensuse.conf
│   │   │   └── mkosi.extra
│   │   │       └── usr
│   │   │           └── lib
│   │   │               ├── encrypted-var.repart.d
│   │   │               │   └── 00-root.conf
│   │   │               └── systemd
│   │   │                   └── system
│   │   │                       ├── encrypted-var.service
│   │   │                       ├── initrd-run-mount.service
│   │   │                       └── initrdcred.service
│   │   ├── minimal-0
│   │   │   ├── mkosi.conf
│   │   │   ├── mkosi.extra
│   │   │   │   ├── opt
│   │   │   │   │   └── some_file
│   │   │   │   └── usr
│   │   │   │       └── lib
│   │   │   │           └── systemd
│   │   │   │               └── system
│   │   │   │                   └── minimal-app0.service
│   │   │   └── mkosi.postinst
│   │   ├── minimal-1
│   │   │   ├── mkosi.conf
│   │   │   ├── mkosi.extra
│   │   │   │   ├── opt
│   │   │   │   │   └── some_file
│   │   │   │   └── usr
│   │   │   │       └── lib
│   │   │   │           └── systemd
│   │   │   │               └── system
│   │   │   │                   └── minimal-app0.service
│   │   │   └── mkosi.postinst
│   │   └── minimal-base
│   │       ├── mkosi.conf
│   │       ├── mkosi.conf.d
│   │       │   ├── arch.conf
│   │       │   ├── build.conf
│   │       │   ├── centos-fedora.conf
│   │       │   ├── debian-ubuntu.conf
│   │       │   └── opensuse.conf
│   │       ├── mkosi.extra
│   │       │   └── etc
│   │       │       └── resolv.conf
│   │       └── mkosi.postinst
│   ├── mkosi.postinst.chroot
│   ├── mkosi.repart
│   │   ├── 00-esp.conf
│   │   ├── 10-root.conf
│   │   └── 20-disk.conf
│   ├── mkosi.sanitizers
│   │   ├── mkosi.conf
│   │   ├── mkosi.conf.d
│   │   │   ├── arch.conf
│   │   │   ├── debian-ubuntu.conf
│   │   │   └── opensuse.conf
│   │   ├── mkosi.extra
│   │   │   └── usr
│   │   │       └── lib
│   │   │           └── systemd
│   │   │               ├── leak-sanitizer-suppressions
│   │   │               ├── system
│   │   │               │   ├── iscsi-init.service.d
│   │   │               │   │   └── 10-asan.conf
│   │   │               │   ├── service.d
│   │   │               │   │   └── 10-timeout-abort.conf
│   │   │               │   ├── systemd-coredump@.service.d
│   │   │               │   │   └── 10-asan.conf
│   │   │               │   └── systemd-journald.service.d
│   │   │               │       └── 10-stdout-tty.conf
│   │   │               └── system.conf.d
│   │   │                   └── 10-sanitizers.conf
│   │   └── mkosi.postinst
│   ├── mkosi.sync
│   ├── mkosi.tools.conf
│   │   ├── mkosi.conf
│   │   └── mkosi.conf.d
│   │       ├── arch.conf
│   │       ├── centos-fedora.conf
│   │       ├── debian-ubuntu.conf
│   │       ├── fedora.conf
│   │       ├── opensuse.conf
│   │       └── ubuntu
│   │           ├── mkosi.conf
│   │           └── mkosi.conf.d
│   │               ├── non-x86.conf
│   │               └── x86.conf
│   ├── mkosi.uki-profiles
│   │   ├── profile1.conf
│   │   └── profile2.conf
│   └── template.cfg
├── modprobe.d
│   ├── meson.build
│   ├── README
│   └── systemd.conf
├── mypy.ini
├── network
│   ├── 80-6rd-tunnel.link
│   ├── 80-6rd-tunnel.network
│   ├── 80-auto-link-local.network.example
│   ├── 80-container-host0-tun.network
│   ├── 80-container-host0.network
│   ├── 80-container-vb.link
│   ├── 80-container-vb.network
│   ├── 80-container-ve.link
│   ├── 80-container-ve.network
│   ├── 80-container-vz.link
│   ├── 80-container-vz.network
│   ├── 80-namespace-ns-tun.link
│   ├── 80-namespace-ns-tun.network
│   ├── 80-namespace-ns.link
│   ├── 80-namespace-ns.network
│   ├── 80-vm-vt.link
│   ├── 80-vm-vt.network
│   ├── 80-wifi-adhoc.network
│   ├── 80-wifi-ap.network.example
│   ├── 80-wifi-station.network.example
│   ├── 89-ethernet.network.example
│   ├── 99-default.link
│   └── meson.build
├── NEWS
├── NOTES-all.md
├── NOTES-dir-only.md
├── po
│   ├── ar.po
│   ├── be.po
│   ├── be@latin.po
│   ├── bg.po
│   ├── ca.po
│   ├── cs.po
│   ├── da.po
│   ├── de.po
│   ├── el.po
│   ├── es.po
│   ├── et.po
│   ├── eu.po
│   ├── fi.po
│   ├── fr.po
│   ├── gl.po
│   ├── he.po
│   ├── hi.po
│   ├── hr.po
│   ├── hu.po
│   ├── ia.po
│   ├── id.po
│   ├── it.po
│   ├── its
│   │   ├── polkit.its
│   │   └── polkit.loc
│   ├── ja.po
│   ├── ka.po
│   ├── kab.po
│   ├── kn.po
│   ├── ko.po
│   ├── LINGUAS
│   ├── lt.po
│   ├── meson.build
│   ├── nl.po
│   ├── pa.po
│   ├── pl.po
│   ├── POTFILES.in
│   ├── POTFILES.skip
│   ├── pt_BR.po
│   ├── pt.po
│   ├── ro.po
│   ├── ru.po
│   ├── si.po
│   ├── sk.po
│   ├── sl.po
│   ├── sr.po
│   ├── sv.po
│   ├── systemd.pot
│   ├── tr.po
│   ├── uk.po
│   ├── zh_CN.po
│   └── zh_TW.po
├── presets
│   ├── 90-systemd-initrd.preset
│   ├── 90-systemd-user.preset
│   ├── 90-systemd.preset
│   ├── 99-default-initrd.preset
│   └── meson.build
├── profile.d
│   ├── 70-systemd-shell-extra.sh
│   ├── 80-systemd-osc-context.sh
│   └── meson.build
├── README
├── README.md
├── ruff.toml
├── rules.d
│   ├── 50-udev-default.rules.in
│   ├── 60-autosuspend.rules
│   ├── 60-block.rules
│   ├── 60-cdrom_id.rules
│   ├── 60-dmi-id.rules
│   ├── 60-drm.rules
│   ├── 60-evdev.rules
│   ├── 60-fido-id.rules
│   ├── 60-infiniband.rules
│   ├── 60-input-id.rules
│   ├── 60-persistent-alsa.rules
│   ├── 60-persistent-hidraw.rules
│   ├── 60-persistent-input.rules
│   ├── 60-persistent-media-controller.rules
│   ├── 60-persistent-storage-mtd.rules
│   ├── 60-persistent-storage-tape.rules
│   ├── 60-persistent-storage.rules.in
│   ├── 60-persistent-v4l.rules
│   ├── 60-sensor.rules
│   ├── 60-serial.rules
│   ├── 64-btrfs.rules.in
│   ├── 70-camera.rules
│   ├── 70-joystick.rules
│   ├── 70-memory.rules
│   ├── 70-mouse.rules
│   ├── 70-power-switch.rules
│   ├── 70-touchpad.rules
│   ├── 70-uaccess.rules.in
│   ├── 71-seat.rules.in
│   ├── 73-seat-late.rules.in
│   ├── 75-net-description.rules
│   ├── 75-probe_mtd.rules
│   ├── 78-sound-card.rules
│   ├── 80-drivers.rules
│   ├── 80-net-setup-link.rules
│   ├── 81-net-bridge.rules
│   ├── 81-net-dhcp.rules
│   ├── 82-net-auto-link-local.rules
│   ├── 90-image-dissect.rules
│   ├── 90-iocost.rules
│   ├── 90-vconsole.rules.in
│   ├── 99-systemd.rules.in
│   ├── meson.build
│   └── README
├── shell-completion
│   ├── bash
│   │   ├── bootctl
│   │   ├── busctl
│   │   ├── coredumpctl
│   │   ├── homectl
│   │   ├── hostnamectl
│   │   ├── importctl
│   │   ├── journalctl
│   │   ├── kernel-install
│   │   ├── localectl
│   │   ├── loginctl
│   │   ├── machinectl
│   │   ├── meson.build
│   │   ├── networkctl
│   │   ├── oomctl
│   │   ├── portablectl
│   │   ├── resolvectl
│   │   ├── run0
│   │   ├── systemctl.in
│   │   ├── systemd-analyze
│   │   ├── systemd-cat
│   │   ├── systemd-cgls
│   │   ├── systemd-cgtop
│   │   ├── systemd-confext
│   │   ├── systemd-creds
│   │   ├── systemd-cryptenroll
│   │   ├── systemd-delta
│   │   ├── systemd-detect-virt
│   │   ├── systemd-dissect
│   │   ├── systemd-id128
│   │   ├── systemd-nspawn
│   │   ├── systemd-path
│   │   ├── systemd-resolve
│   │   ├── systemd-run
│   │   ├── systemd-sysext
│   │   ├── systemd-vmspawn
│   │   ├── systemd-vpick
│   │   ├── timedatectl
│   │   ├── udevadm
│   │   └── userdbctl
│   └── zsh
│       ├── _bootctl
│       ├── _busctl
│       ├── _coredumpctl
│       ├── _hostnamectl
│       ├── _journalctl
│       ├── _kernel-install
│       ├── _localectl
│       ├── _loginctl
│       ├── _machinectl
│       ├── _networkctl
│       ├── _oomctl
│       ├── _resolvectl
│       ├── _run0
│       ├── _sd_hosts_or_user_at_host
│       ├── _sd_machines
│       ├── _sd_outputmodes
│       ├── _sd_unit_files
│       ├── _systemctl.in
│       ├── _systemd
│       ├── _systemd-analyze
│       ├── _systemd-delta
│       ├── _systemd-inhibit
│       ├── _systemd-nspawn
│       ├── _systemd-path
│       ├── _systemd-run
│       ├── _systemd-tmpfiles
│       ├── _timedatectl
│       ├── _udevadm
│       ├── _varlinkctl
│       └── meson.build
├── src
│   ├── ac-power
│   │   ├── ac-power.c
│   │   └── meson.build
│   ├── analyze
│   │   ├── analyze-architectures.c
│   │   ├── analyze-architectures.h
│   │   ├── analyze-blame.c
│   │   ├── analyze-blame.h
│   │   ├── analyze-calendar.c
│   │   ├── analyze-calendar.h
│   │   ├── analyze-capability.c
│   │   ├── analyze-capability.h
│   │   ├── analyze-cat-config.c
│   │   ├── analyze-cat-config.h
│   │   ├── analyze-chid.c
│   │   ├── analyze-chid.h
│   │   ├── analyze-compare-versions.c
│   │   ├── analyze-compare-versions.h
│   │   ├── analyze-condition.c
│   │   ├── analyze-condition.h
│   │   ├── analyze-critical-chain.c
│   │   ├── analyze-critical-chain.h
│   │   ├── analyze-dot.c
│   │   ├── analyze-dot.h
│   │   ├── analyze-dump.c
│   │   ├── analyze-dump.h
│   │   ├── analyze-exit-status.c
│   │   ├── analyze-exit-status.h
│   │   ├── analyze-fdstore.c
│   │   ├── analyze-fdstore.h
│   │   ├── analyze-filesystems.c
│   │   ├── analyze-filesystems.h
│   │   ├── analyze-has-tpm2.c
│   │   ├── analyze-has-tpm2.h
│   │   ├── analyze-image-policy.c
│   │   ├── analyze-image-policy.h
│   │   ├── analyze-inspect-elf.c
│   │   ├── analyze-inspect-elf.h
│   │   ├── analyze-log-control.c
│   │   ├── analyze-log-control.h
│   │   ├── analyze-malloc.c
│   │   ├── analyze-malloc.h
│   │   ├── analyze-pcrs.c
│   │   ├── analyze-pcrs.h
│   │   ├── analyze-plot.c
│   │   ├── analyze-plot.h
│   │   ├── analyze-security.c
│   │   ├── analyze-security.h
│   │   ├── analyze-service-watchdogs.c
│   │   ├── analyze-service-watchdogs.h
│   │   ├── analyze-smbios11.c
│   │   ├── analyze-smbios11.h
│   │   ├── analyze-srk.c
│   │   ├── analyze-srk.h
│   │   ├── analyze-syscall-filter.c
│   │   ├── analyze-syscall-filter.h
│   │   ├── analyze-time-data.c
│   │   ├── analyze-time-data.h
│   │   ├── analyze-time.c
│   │   ├── analyze-time.h
│   │   ├── analyze-timespan.c
│   │   ├── analyze-timespan.h
│   │   ├── analyze-timestamp.c
│   │   ├── analyze-timestamp.h
│   │   ├── analyze-unit-files.c
│   │   ├── analyze-unit-files.h
│   │   ├── analyze-unit-paths.c
│   │   ├── analyze-unit-paths.h
│   │   ├── analyze-unit-shell.c
│   │   ├── analyze-unit-shell.h
│   │   ├── analyze-verify-util.c
│   │   ├── analyze-verify-util.h
│   │   ├── analyze-verify.c
│   │   ├── analyze-verify.h
│   │   ├── analyze.c
│   │   ├── analyze.h
│   │   ├── meson.build
│   │   └── test-verify.c
│   ├── ask-password
│   │   ├── ask-password.c
│   │   ├── io.systemd.ask-password.policy
│   │   └── meson.build
│   ├── backlight
│   │   ├── backlight.c
│   │   └── meson.build
│   ├── basic
│   │   ├── af-list.c
│   │   ├── af-list.h
│   │   ├── af-to-name.awk
│   │   ├── alloc-util.c
│   │   ├── alloc-util.h
│   │   ├── ansi-color.c
│   │   ├── ansi-color.h
│   │   ├── architecture.c
│   │   ├── architecture.h
│   │   ├── argv-util.c
│   │   ├── argv-util.h
│   │   ├── arphrd-to-name.awk
│   │   ├── arphrd-util.c
│   │   ├── arphrd-util.h
│   │   ├── assert-util.c
│   │   ├── assert-util.h
│   │   ├── audit-util.c
│   │   ├── audit-util.h
│   │   ├── bitfield.h
│   │   ├── btrfs.c
│   │   ├── btrfs.h
│   │   ├── build-path.c
│   │   ├── build-path.h
│   │   ├── build.c
│   │   ├── build.h
│   │   ├── bus-label.c
│   │   ├── bus-label.h
│   │   ├── capability-list.c
│   │   ├── capability-list.h
│   │   ├── capability-to-name.awk
│   │   ├── capability-util.c
│   │   ├── capability-util.h
│   │   ├── capsule-util.c
│   │   ├── capsule-util.h
│   │   ├── cgroup-util.c
│   │   ├── cgroup-util.h
│   │   ├── chase.c
│   │   ├── chase.h
│   │   ├── chattr-util.c
│   │   ├── chattr-util.h
│   │   ├── check-filesystems.sh
│   │   ├── cleanup-util.h
│   │   ├── compress.c
│   │   ├── compress.h
│   │   ├── conf-files.c
│   │   ├── conf-files.h
│   │   ├── confidential-virt.c
│   │   ├── confidential-virt.h
│   │   ├── constants.h
│   │   ├── devnum-util.c
│   │   ├── devnum-util.h
│   │   ├── dirent-util.c
│   │   ├── dirent-util.h
│   │   ├── dlfcn-util.c
│   │   ├── dlfcn-util.h
│   │   ├── dns-def.h
│   │   ├── efivars.c
│   │   ├── efivars.h
│   │   ├── env-file.c
│   │   ├── env-file.h
│   │   ├── env-util.c
│   │   ├── env-util.h
│   │   ├── errno-list.c
│   │   ├── errno-list.h
│   │   ├── errno-to-name.awk
│   │   ├── errno-util.h
│   │   ├── escape.c
│   │   ├── escape.h
│   │   ├── ether-addr-util.c
│   │   ├── ether-addr-util.h
│   │   ├── extract-word.c
│   │   ├── extract-word.h
│   │   ├── fd-util.c
│   │   ├── fd-util.h
│   │   ├── fileio.c
│   │   ├── fileio.h
│   │   ├── filesystems-gperf.gperf
│   │   ├── filesystems.c
│   │   ├── filesystems.h
│   │   ├── format-ifname.c
│   │   ├── format-ifname.h
│   │   ├── format-util.c
│   │   ├── format-util.h
│   │   ├── forward.h
│   │   ├── fs-util.c
│   │   ├── fs-util.h
│   │   ├── gcrypt-util.c
│   │   ├── gcrypt-util.h
│   │   ├── generate-af-list.sh
│   │   ├── generate-arphrd-list.sh
│   │   ├── generate-capability-list.sh
│   │   ├── generate-errno-list.sh
│   │   ├── generate-filesystem-list.py
│   │   ├── generate-filesystem-switch-case.py
│   │   ├── getopt-defs.h
│   │   ├── glob-util.c
│   │   ├── glob-util.h
│   │   ├── glyph-util.c
│   │   ├── glyph-util.h
│   │   ├── gunicode.c
│   │   ├── gunicode.h
│   │   ├── hash-funcs.c
│   │   ├── hash-funcs.h
│   │   ├── hashmap.c
│   │   ├── hashmap.h
│   │   ├── hexdecoct.c
│   │   ├── hexdecoct.h
│   │   ├── hmac.c
│   │   ├── hmac.h
│   │   ├── hostname-util.c
│   │   ├── hostname-util.h
│   │   ├── in-addr-util.c
│   │   ├── in-addr-util.h
│   │   ├── initrd-util.c
│   │   ├── initrd-util.h
│   │   ├── inotify-util.c
│   │   ├── inotify-util.h
│   │   ├── io-util.c
│   │   ├── io-util.h
│   │   ├── iovec-util.c
│   │   ├── iovec-util.h
│   │   ├── iovec-wrapper.c
│   │   ├── iovec-wrapper.h
│   │   ├── iterator.h
│   │   ├── keyring-util.c
│   │   ├── keyring-util.h
│   │   ├── label.c
│   │   ├── label.h
│   │   ├── limits-util.c
│   │   ├── limits-util.h
│   │   ├── list.h
│   │   ├── locale-util.c
│   │   ├── locale-util.h
│   │   ├── lock-util.c
│   │   ├── lock-util.h
│   │   ├── log-context.c
│   │   ├── log-context.h
│   │   ├── log-ratelimit.h
│   │   ├── log.c
│   │   ├── log.h
│   │   ├── login-util.c
│   │   ├── login-util.h
│   │   ├── macro.h
│   │   ├── math-util.h
│   │   ├── memfd-util.c
│   │   ├── memfd-util.h
│   │   ├── memory-util.c
│   │   ├── memory-util.h
│   │   ├── mempool.c
│   │   ├── mempool.h
│   │   ├── memstream-util.c
│   │   ├── memstream-util.h
│   │   ├── meson.build
│   │   ├── missing-drm.h
│   │   ├── missing-network.h
│   │   ├── mkdir.c
│   │   ├── mkdir.h
│   │   ├── mountpoint-util.c
│   │   ├── mountpoint-util.h
│   │   ├── MurmurHash2.c
│   │   ├── MurmurHash2.h
│   │   ├── namespace-util.c
│   │   ├── namespace-util.h
│   │   ├── nss-util.h
│   │   ├── nulstr-util.c
│   │   ├── nulstr-util.h
│   │   ├── ordered-set.c
│   │   ├── ordered-set.h
│   │   ├── origin-id.h
│   │   ├── os-util.c
│   │   ├── os-util.h
│   │   ├── parse-util.c
│   │   ├── parse-util.h
│   │   ├── path-util.c
│   │   ├── path-util.h
│   │   ├── pcapng.h
│   │   ├── percent-util.c
│   │   ├── percent-util.h
│   │   ├── pidfd-util.c
│   │   ├── pidfd-util.h
│   │   ├── pidref.c
│   │   ├── pidref.h
│   │   ├── prioq.c
│   │   ├── prioq.h
│   │   ├── proc-cmdline.c
│   │   ├── proc-cmdline.h
│   │   ├── process-util.c
│   │   ├── process-util.h
│   │   ├── procfs-util.c
│   │   ├── procfs-util.h
│   │   ├── psi-util.c
│   │   ├── psi-util.h
│   │   ├── pthread-util.h
│   │   ├── random-util.c
│   │   ├── random-util.h
│   │   ├── ratelimit.c
│   │   ├── ratelimit.h
│   │   ├── raw-clone.c
│   │   ├── raw-clone.h
│   │   ├── recurse-dir.c
│   │   ├── recurse-dir.h
│   │   ├── replace-var.c
│   │   ├── replace-var.h
│   │   ├── rlimit-util.c
│   │   ├── rlimit-util.h
│   │   ├── runtime-scope.c
│   │   ├── runtime-scope.h
│   │   ├── set.h
│   │   ├── sha256.c
│   │   ├── sha256.h
│   │   ├── sigbus.c
│   │   ├── sigbus.h
│   │   ├── signal-util.c
│   │   ├── signal-util.h
│   │   ├── siphash24.c
│   │   ├── siphash24.h
│   │   ├── socket-util.c
│   │   ├── socket-util.h
│   │   ├── sort-util.c
│   │   ├── sort-util.h
│   │   ├── sparse-endian.h
│   │   ├── special.h
│   │   ├── stat-util.c
│   │   ├── stat-util.h
│   │   ├── static-destruct.c
│   │   ├── static-destruct.h
│   │   ├── stdio-util.h
│   │   ├── strbuf.c
│   │   ├── strbuf.h
│   │   ├── string-table.c
│   │   ├── string-table.h
│   │   ├── string-util.c
│   │   ├── string-util.h
│   │   ├── strv.c
│   │   ├── strv.h
│   │   ├── strxcpyx.c
│   │   ├── strxcpyx.h
│   │   ├── sync-util.c
│   │   ├── sync-util.h
│   │   ├── sysctl-util.c
│   │   ├── sysctl-util.h
│   │   ├── syslog-util.c
│   │   ├── syslog-util.h
│   │   ├── terminal-util.c
│   │   ├── terminal-util.h
│   │   ├── time-util.c
│   │   ├── time-util.h
│   │   ├── tmpfile-util.c
│   │   ├── tmpfile-util.h
│   │   ├── uid-classification.c
│   │   ├── uid-classification.h
│   │   ├── uid-range.c
│   │   ├── uid-range.h
│   │   ├── umask-util.h
│   │   ├── unaligned.h
│   │   ├── unit-def.c
│   │   ├── unit-def.h
│   │   ├── unit-name.c
│   │   ├── unit-name.h
│   │   ├── user-util.c
│   │   ├── user-util.h
│   │   ├── utf8.c
│   │   ├── utf8.h
│   │   ├── virt.c
│   │   ├── virt.h
│   │   ├── xattr-util.c
│   │   └── xattr-util.h
│   ├── battery-check
│   │   ├── battery-check.c
│   │   └── meson.build
│   ├── binfmt
│   │   ├── binfmt.c
│   │   └── meson.build
│   ├── bless-boot
│   │   ├── bless-boot-generator.c
│   │   ├── bless-boot.c
│   │   ├── boot-check-no-failures.c
│   │   └── meson.build
│   ├── boot
│   │   ├── addon.c
│   │   ├── bcd.c
│   │   ├── bcd.h
│   │   ├── boot.c
│   │   ├── chid.c
│   │   ├── chid.h
│   │   ├── console.c
│   │   ├── console.h
│   │   ├── cpio.c
│   │   ├── cpio.h
│   │   ├── device-path-util.c
│   │   ├── device-path-util.h
│   │   ├── devicetree.c
│   │   ├── devicetree.h
│   │   ├── drivers.c
│   │   ├── drivers.h
│   │   ├── edid.c
│   │   ├── edid.h
│   │   ├── efi-efivars.c
│   │   ├── efi-efivars.h
│   │   ├── efi-firmware.c
│   │   ├── efi-firmware.h
│   │   ├── efi-log.c
│   │   ├── efi-log.h
│   │   ├── efi-string-table.h
│   │   ├── efi-string.c
│   │   ├── efi-string.h
│   │   ├── efi.h
│   │   ├── export-vars.c
│   │   ├── export-vars.h
│   │   ├── fuzz-bcd.c
│   │   ├── fuzz-efi-osrel.c
│   │   ├── fuzz-efi-printf.c
│   │   ├── fuzz-efi-string.c
│   │   ├── generate-hwids-section.py
│   │   ├── graphics.c
│   │   ├── graphics.h
│   │   ├── hwids
│   │   │   ├── device1.json
│   │   │   ├── device2.json
│   │   │   ├── device3.json
│   │   │   └── device4.json
│   │   ├── initrd.c
│   │   ├── initrd.h
│   │   ├── line-edit.c
│   │   ├── line-edit.h
│   │   ├── linux_x86.c
│   │   ├── linux.c
│   │   ├── linux.h
│   │   ├── measure.c
│   │   ├── measure.h
│   │   ├── meson.build
│   │   ├── part-discovery.c
│   │   ├── part-discovery.h
│   │   ├── pe.c
│   │   ├── pe.h
│   │   ├── proto
│   │   │   ├── block-io.h
│   │   │   ├── cc-measurement.h
│   │   │   ├── console-control.h
│   │   │   ├── device-path.h
│   │   │   ├── dt-fixup.h
│   │   │   ├── edid-discovered.h
│   │   │   ├── file-io.h
│   │   │   ├── graphics-output.h
│   │   │   ├── load-file.h
│   │   │   ├── loaded-image.h
│   │   │   ├── rng.h
│   │   │   ├── security-arch.h
│   │   │   ├── shell-parameters.h
│   │   │   ├── simple-text-io.h
│   │   │   └── tcg.h
│   │   ├── random-seed.c
│   │   ├── random-seed.h
│   │   ├── secure-boot.c
│   │   ├── secure-boot.h
│   │   ├── shim.c
│   │   ├── shim.h
│   │   ├── smbios.c
│   │   ├── smbios.h
│   │   ├── splash.c
│   │   ├── splash.h
│   │   ├── stub.c
│   │   ├── sysfail.c
│   │   ├── sysfail.h
│   │   ├── test-bcd.c
│   │   ├── test-chid-match.c
│   │   ├── test-efi-string.c
│   │   ├── ticks.c
│   │   ├── ticks.h
│   │   ├── ubsan.c
│   │   ├── UEFI_SECURITY.md
│   │   ├── url-discovery.c
│   │   ├── url-discovery.h
│   │   ├── util.c
│   │   ├── util.h
│   │   ├── vmm.c
│   │   └── vmm.h
│   ├── bootctl
│   │   ├── bootctl-install.c
│   │   ├── bootctl-install.h
│   │   ├── bootctl-random-seed.c
│   │   ├── bootctl-random-seed.h
│   │   ├── bootctl-reboot-to-firmware.c
│   │   ├── bootctl-reboot-to-firmware.h
│   │   ├── bootctl-set-efivar.c
│   │   ├── bootctl-set-efivar.h
│   │   ├── bootctl-status.c
│   │   ├── bootctl-status.h
│   │   ├── bootctl-uki.c
│   │   ├── bootctl-uki.h
│   │   ├── bootctl-util.c
│   │   ├── bootctl-util.h
│   │   ├── bootctl.c
│   │   ├── bootctl.h
│   │   └── meson.build
│   ├── busctl
│   │   ├── busctl-introspect.c
│   │   ├── busctl-introspect.h
│   │   ├── busctl.c
│   │   ├── meson.build
│   │   └── test-busctl-introspect.c
│   ├── cgls
│   │   ├── cgls.c
│   │   └── meson.build
│   ├── cgtop
│   │   ├── cgtop.c
│   │   └── meson.build
│   ├── core
│   │   ├── all-units.h
│   │   ├── apparmor-setup.c
│   │   ├── apparmor-setup.h
│   │   ├── audit-fd.c
│   │   ├── audit-fd.h
│   │   ├── automount.c
│   │   ├── automount.h
│   │   ├── bpf
│   │   │   ├── restrict-fs
│   │   │   │   ├── meson.build
│   │   │   │   ├── restrict-fs-skel.h
│   │   │   │   └── restrict-fs.bpf.c
│   │   │   ├── restrict-ifaces
│   │   │   │   ├── meson.build
│   │   │   │   ├── restrict-ifaces-skel.h
│   │   │   │   └── restrict-ifaces.bpf.c
│   │   │   └── socket-bind
│   │   │       ├── meson.build
│   │   │       ├── socket-bind-api.bpf.h
│   │   │       ├── socket-bind-skel.h
│   │   │       └── socket-bind.bpf.c
│   │   ├── bpf-devices.c
│   │   ├── bpf-devices.h
│   │   ├── bpf-firewall.c
│   │   ├── bpf-firewall.h
│   │   ├── bpf-foreign.c
│   │   ├── bpf-foreign.h
│   │   ├── bpf-restrict-fs.c
│   │   ├── bpf-restrict-fs.h
│   │   ├── bpf-restrict-ifaces.c
│   │   ├── bpf-restrict-ifaces.h
│   │   ├── bpf-socket-bind.c
│   │   ├── bpf-socket-bind.h
│   │   ├── cgroup.c
│   │   ├── cgroup.h
│   │   ├── clock-warp.c
│   │   ├── clock-warp.h
│   │   ├── core-forward.h
│   │   ├── crash-handler.c
│   │   ├── crash-handler.h
│   │   ├── dbus-automount.c
│   │   ├── dbus-automount.h
│   │   ├── dbus-cgroup.c
│   │   ├── dbus-cgroup.h
│   │   ├── dbus-device.c
│   │   ├── dbus-device.h
│   │   ├── dbus-execute.c
│   │   ├── dbus-execute.h
│   │   ├── dbus-job.c
│   │   ├── dbus-job.h
│   │   ├── dbus-kill.c
│   │   ├── dbus-kill.h
│   │   ├── dbus-manager.c
│   │   ├── dbus-manager.h
│   │   ├── dbus-mount.c
│   │   ├── dbus-mount.h
│   │   ├── dbus-path.c
│   │   ├── dbus-path.h
│   │   ├── dbus-scope.c
│   │   ├── dbus-scope.h
│   │   ├── dbus-service.c
│   │   ├── dbus-service.h
│   │   ├── dbus-slice.c
│   │   ├── dbus-slice.h
│   │   ├── dbus-socket.c
│   │   ├── dbus-socket.h
│   │   ├── dbus-swap.c
│   │   ├── dbus-swap.h
│   │   ├── dbus-target.c
│   │   ├── dbus-target.h
│   │   ├── dbus-timer.c
│   │   ├── dbus-timer.h
│   │   ├── dbus-unit.c
│   │   ├── dbus-unit.h
│   │   ├── dbus-util.c
│   │   ├── dbus-util.h
│   │   ├── dbus.c
│   │   ├── dbus.h
│   │   ├── device.c
│   │   ├── device.h
│   │   ├── dynamic-user.c
│   │   ├── dynamic-user.h
│   │   ├── efi-random.c
│   │   ├── efi-random.h
│   │   ├── emergency-action.c
│   │   ├── emergency-action.h
│   │   ├── exec-credential.c
│   │   ├── exec-credential.h
│   │   ├── exec-invoke.c
│   │   ├── exec-invoke.h
│   │   ├── execute-serialize.c
│   │   ├── execute-serialize.h
│   │   ├── execute.c
│   │   ├── execute.h
│   │   ├── executor.c
│   │   ├── fuzz-execute-serialize.c
│   │   ├── fuzz-manager-serialize.c
│   │   ├── fuzz-manager-serialize.options
│   │   ├── fuzz-unit-file.c
│   │   ├── fuzz-unit-file.options
│   │   ├── generate-bpf-delegate-configs.py
│   │   ├── generator-setup.c
│   │   ├── generator-setup.h
│   │   ├── ima-setup.c
│   │   ├── ima-setup.h
│   │   ├── import-creds.c
│   │   ├── import-creds.h
│   │   ├── ipe-setup.c
│   │   ├── ipe-setup.h
│   │   ├── job.c
│   │   ├── job.h
│   │   ├── kill.c
│   │   ├── kill.h
│   │   ├── kmod-setup.c
│   │   ├── kmod-setup.h
│   │   ├── load-dropin.c
│   │   ├── load-dropin.h
│   │   ├── load-fragment-gperf-nulstr.awk
│   │   ├── load-fragment-gperf.gperf.in
│   │   ├── load-fragment.c
│   │   ├── load-fragment.h
│   │   ├── main.c
│   │   ├── main.h
│   │   ├── manager-dump.c
│   │   ├── manager-dump.h
│   │   ├── manager-serialize.c
│   │   ├── manager-serialize.h
│   │   ├── manager.c
│   │   ├── manager.h
│   │   ├── meson.build
│   │   ├── mount.c
│   │   ├── mount.h
│   │   ├── namespace.c
│   │   ├── namespace.h
│   │   ├── org.freedesktop.systemd1.conf
│   │   ├── org.freedesktop.systemd1.policy.in
│   │   ├── org.freedesktop.systemd1.service
│   │   ├── path.c
│   │   ├── path.h
│   │   ├── scope.c
│   │   ├── scope.h
│   │   ├── selinux-access.c
│   │   ├── selinux-access.h
│   │   ├── selinux-setup.c
│   │   ├── selinux-setup.h
│   │   ├── service.c
│   │   ├── service.h
│   │   ├── show-status.c
│   │   ├── show-status.h
│   │   ├── slice.c
│   │   ├── slice.h
│   │   ├── smack-setup.c
│   │   ├── smack-setup.h
│   │   ├── socket.c
│   │   ├── socket.h
│   │   ├── swap.c
│   │   ├── swap.h
│   │   ├── system.conf.in
│   │   ├── systemd.pc.in
│   │   ├── taint.c
│   │   ├── taint.h
│   │   ├── target.c
│   │   ├── target.h
│   │   ├── timer.c
│   │   ├── timer.h
│   │   ├── transaction.c
│   │   ├── transaction.h
│   │   ├── unit-dependency-atom.c
│   │   ├── unit-dependency-atom.h
│   │   ├── unit-printf.c
│   │   ├── unit-printf.h
│   │   ├── unit-serialize.c
│   │   ├── unit-serialize.h
│   │   ├── unit.c
│   │   ├── unit.h
│   │   ├── user.conf.in
│   │   ├── varlink-cgroup.c
│   │   ├── varlink-cgroup.h
│   │   ├── varlink-common.c
│   │   ├── varlink-common.h
│   │   ├── varlink-dynamic-user.c
│   │   ├── varlink-dynamic-user.h
│   │   ├── varlink-manager.c
│   │   ├── varlink-manager.h
│   │   ├── varlink-unit.c
│   │   ├── varlink-unit.h
│   │   ├── varlink.c
│   │   └── varlink.h
│   ├── coredump
│   │   ├── coredump-vacuum.c
│   │   ├── coredump-vacuum.h
│   │   ├── coredump.c
│   │   ├── coredump.conf
│   │   ├── coredumpctl.c
│   │   ├── meson.build
│   │   └── test-coredump-vacuum.c
│   ├── coverage
│   │   ├── coverage.h
│   │   └── meson.build
│   ├── creds
│   │   ├── creds.c
│   │   ├── io.systemd.credentials.policy
│   │   └── meson.build
│   ├── cryptenroll
│   │   ├── cryptenroll-fido2.c
│   │   ├── cryptenroll-fido2.h
│   │   ├── cryptenroll-list.c
│   │   ├── cryptenroll-list.h
│   │   ├── cryptenroll-password.c
│   │   ├── cryptenroll-password.h
│   │   ├── cryptenroll-pkcs11.c
│   │   ├── cryptenroll-pkcs11.h
│   │   ├── cryptenroll-recovery.c
│   │   ├── cryptenroll-recovery.h
│   │   ├── cryptenroll-tpm2.c
│   │   ├── cryptenroll-tpm2.h
│   │   ├── cryptenroll-wipe.c
│   │   ├── cryptenroll-wipe.h
│   │   ├── cryptenroll.c
│   │   ├── cryptenroll.h
│   │   └── meson.build
│   ├── cryptsetup
│   │   ├── cryptsetup-generator.c
│   │   ├── cryptsetup-keyfile.c
│   │   ├── cryptsetup-keyfile.h
│   │   ├── cryptsetup-pkcs11.c
│   │   ├── cryptsetup-pkcs11.h
│   │   ├── cryptsetup-tokens
│   │   │   ├── cryptsetup-token-systemd-fido2.c
│   │   │   ├── cryptsetup-token-systemd-pkcs11.c
│   │   │   ├── cryptsetup-token-systemd-tpm2.c
│   │   │   ├── cryptsetup-token-util.c
│   │   │   ├── cryptsetup-token-util.h
│   │   │   ├── cryptsetup-token.h
│   │   │   ├── cryptsetup-token.sym
│   │   │   ├── luks2-fido2.c
│   │   │   ├── luks2-fido2.h
│   │   │   ├── luks2-pkcs11.c
│   │   │   ├── luks2-pkcs11.h
│   │   │   ├── luks2-tpm2.c
│   │   │   ├── luks2-tpm2.h
│   │   │   └── meson.build
│   │   ├── cryptsetup.c
│   │   └── meson.build
│   ├── debug-generator
│   │   ├── debug-generator.c
│   │   └── meson.build
│   ├── delta
│   │   ├── delta.c
│   │   └── meson.build
│   ├── detect-virt
│   │   ├── detect-virt.c
│   │   └── meson.build
│   ├── dissect
│   │   ├── dissect.c
│   │   └── meson.build
│   ├── environment-d-generator
│   │   ├── environment-d-generator.c
│   │   └── meson.build
│   ├── escape
│   │   ├── escape-tool.c
│   │   └── meson.build
│   ├── factory-reset
│   │   ├── factory-reset-generator.c
│   │   ├── factory-reset-tool.c
│   │   └── meson.build
│   ├── firstboot
│   │   ├── firstboot.c
│   │   └── meson.build
│   ├── fsck
│   │   ├── fsck.c
│   │   └── meson.build
│   ├── fstab-generator
│   │   ├── fstab-generator.c
│   │   └── meson.build
│   ├── fundamental
│   │   ├── assert-fundamental.h
│   │   ├── bootspec-fundamental.c
│   │   ├── bootspec-fundamental.h
│   │   ├── chid-fundamental.c
│   │   ├── chid-fundamental.h
│   │   ├── cleanup-fundamental.h
│   │   ├── confidential-virt-fundamental.h
│   │   ├── edid-fundamental.c
│   │   ├── edid-fundamental.h
│   │   ├── efi-fundamental.h
│   │   ├── efivars-fundamental.c
│   │   ├── efivars-fundamental.h
│   │   ├── iovec-util-fundamental.h
│   │   ├── logarithm.h
│   │   ├── macro-fundamental.h
│   │   ├── memory-util-fundamental.h
│   │   ├── meson.build
│   │   ├── sbat.h
│   │   ├── sha1-fundamental.c
│   │   ├── sha1-fundamental.h
│   │   ├── sha256-fundamental.c
│   │   ├── sha256-fundamental.h
│   │   ├── string-util-fundamental.c
│   │   ├── string-util-fundamental.h
│   │   ├── strv-fundamental.h
│   │   ├── tpm2-pcr.h
│   │   ├── uki.c
│   │   ├── uki.h
│   │   └── unaligned-fundamental.h
│   ├── fuzz
│   │   ├── fuzz-bootspec-gen.py
│   │   ├── fuzz-bootspec.c
│   │   ├── fuzz-bootspec.options
│   │   ├── fuzz-bus-label.c
│   │   ├── fuzz-calendarspec.c
│   │   ├── fuzz-catalog.c
│   │   ├── fuzz-compress.c
│   │   ├── fuzz-env-file.c
│   │   ├── fuzz-env-file.options
│   │   ├── fuzz-hostname-setup.c
│   │   ├── fuzz-json.c
│   │   ├── fuzz-main.c
│   │   ├── fuzz-time-util.c
│   │   ├── fuzz-udev-database.c
│   │   ├── fuzz-varlink-idl.c
│   │   ├── fuzz-varlink.c
│   │   ├── fuzz.h
│   │   └── meson.build
│   ├── getty-generator
│   │   ├── getty-generator.c
│   │   └── meson.build
│   ├── gpt-auto-generator
│   │   ├── gpt-auto-generator.c
│   │   └── meson.build
│   ├── growfs
│   │   ├── growfs.c
│   │   ├── makefs.c
│   │   └── meson.build
│   ├── hibernate-resume
│   │   ├── hibernate-resume-config.c
│   │   ├── hibernate-resume-config.h
│   │   ├── hibernate-resume-generator.c
│   │   ├── hibernate-resume.c
│   │   └── meson.build
│   ├── home
│   │   ├── home-util.c
│   │   ├── home-util.h
│   │   ├── homectl-fido2.c
│   │   ├── homectl-fido2.h
│   │   ├── homectl-pkcs11.c
│   │   ├── homectl-pkcs11.h
│   │   ├── homectl-recovery-key.c
│   │   ├── homectl-recovery-key.h
│   │   ├── homectl.c
│   │   ├── homed-bus.c
│   │   ├── homed-bus.h
│   │   ├── homed-conf.c
│   │   ├── homed-conf.h
│   │   ├── homed-forward.h
│   │   ├── homed-gperf.gperf
│   │   ├── homed-home-bus.c
│   │   ├── homed-home-bus.h
│   │   ├── homed-home.c
│   │   ├── homed-home.h
│   │   ├── homed-manager-bus.c
│   │   ├── homed-manager-bus.h
│   │   ├── homed-manager.c
│   │   ├── homed-manager.h
│   │   ├── homed-operation.c
│   │   ├── homed-operation.h
│   │   ├── homed-varlink.c
│   │   ├── homed-varlink.h
│   │   ├── homed.c
│   │   ├── homed.conf
│   │   ├── homework-blob.c
│   │   ├── homework-blob.h
│   │   ├── homework-cifs.c
│   │   ├── homework-cifs.h
│   │   ├── homework-directory.c
│   │   ├── homework-directory.h
│   │   ├── homework-fido2.c
│   │   ├── homework-fido2.h
│   │   ├── homework-forward.h
│   │   ├── homework-fscrypt.c
│   │   ├── homework-fscrypt.h
│   │   ├── homework-luks.c
│   │   ├── homework-luks.h
│   │   ├── homework-mount.c
│   │   ├── homework-mount.h
│   │   ├── homework-password-cache.c
│   │   ├── homework-password-cache.h
│   │   ├── homework-pkcs11.c
│   │   ├── homework-pkcs11.h
│   │   ├── homework-quota.c
│   │   ├── homework-quota.h
│   │   ├── homework.c
│   │   ├── homework.h
│   │   ├── meson.build
│   │   ├── org.freedesktop.home1.conf
│   │   ├── org.freedesktop.home1.policy
│   │   ├── org.freedesktop.home1.service
│   │   ├── pam_systemd_home.c
│   │   ├── pam_systemd_home.sym
│   │   ├── test-homed-regression-31896.c
│   │   ├── user-record-password-quality.c
│   │   ├── user-record-password-quality.h
│   │   ├── user-record-sign.c
│   │   ├── user-record-sign.h
│   │   ├── user-record-util.c
│   │   └── user-record-util.h
│   ├── hostname
│   │   ├── hostnamectl.c
│   │   ├── hostnamed.c
│   │   ├── meson.build
│   │   ├── org.freedesktop.hostname1.conf
│   │   ├── org.freedesktop.hostname1.policy
│   │   └── org.freedesktop.hostname1.service
│   ├── hwdb
│   │   ├── hwdb.c
│   │   └── meson.build
│   ├── id128
│   │   ├── id128.c
│   │   └── meson.build
│   ├── import
│   │   ├── curl-util.c
│   │   ├── curl-util.h
│   │   ├── export-raw.c
│   │   ├── export-raw.h
│   │   ├── export-tar.c
│   │   ├── export-tar.h
│   │   ├── export.c
│   │   ├── import-common.c
│   │   ├── import-common.h
│   │   ├── import-compress.c
│   │   ├── import-compress.h
│   │   ├── import-fs.c
│   │   ├── import-generator.c
│   │   ├── import-pubring.pgp
│   │   ├── import-raw.c
│   │   ├── import-raw.h
│   │   ├── import-tar.c
│   │   ├── import-tar.h
│   │   ├── import.c
│   │   ├── importctl.c
│   │   ├── importd.c
│   │   ├── meson.build
│   │   ├── org.freedesktop.import1.conf
│   │   ├── org.freedesktop.import1.policy
│   │   ├── org.freedesktop.import1.service
│   │   ├── pull-common.c
│   │   ├── pull-common.h
│   │   ├── pull-job.c
│   │   ├── pull-job.h
│   │   ├── pull-raw.c
│   │   ├── pull-raw.h
│   │   ├── pull-tar.c
│   │   ├── pull-tar.h
│   │   ├── pull.c
│   │   ├── qcow2-util.c
│   │   ├── qcow2-util.h
│   │   └── test-qcow2.c
│   ├── include
│   │   ├── meson.build
│   │   ├── override
│   │   │   ├── fcntl.h
│   │   │   ├── linux
│   │   │   │   ├── audit.h
│   │   │   │   ├── bpf.h
│   │   │   │   ├── fs.h
│   │   │   │   ├── keyctl.h
│   │   │   │   ├── magic.h
│   │   │   │   ├── nsfs.h
│   │   │   │   └── xfs.h
│   │   │   ├── malloc.h
│   │   │   ├── net
│   │   │   │   ├── if_arp.h
│   │   │   │   └── if.h
│   │   │   ├── netinet
│   │   │   │   └── in.h
│   │   │   ├── sched.h
│   │   │   ├── signal.h
│   │   │   ├── sys
│   │   │   │   ├── bpf.h
│   │   │   │   ├── generate-syscall.py
│   │   │   │   ├── ioprio.h
│   │   │   │   ├── kcmp.h
│   │   │   │   ├── keyctl.h
│   │   │   │   ├── mempolicy.h
│   │   │   │   ├── meson.build
│   │   │   │   ├── mman.h
│   │   │   │   ├── mount.h
│   │   │   │   ├── param.h
│   │   │   │   ├── pidfd.h
│   │   │   │   ├── quota.h
│   │   │   │   ├── random.h
│   │   │   │   ├── socket.h
│   │   │   │   ├── stat.h
│   │   │   │   ├── syscall-list.txt
│   │   │   │   ├── syscall.h
│   │   │   │   ├── syscalls-alpha.txt
│   │   │   │   ├── syscalls-arc.txt
│   │   │   │   ├── syscalls-arm.txt
│   │   │   │   ├── syscalls-arm64.txt
│   │   │   │   ├── syscalls-i386.txt
│   │   │   │   ├── syscalls-ia64.txt
│   │   │   │   ├── syscalls-loongarch64.txt
│   │   │   │   ├── syscalls-m68k.txt
│   │   │   │   ├── syscalls-mips64.txt
│   │   │   │   ├── syscalls-mips64n32.txt
│   │   │   │   ├── syscalls-mipso32.txt
│   │   │   │   ├── syscalls-parisc.txt
│   │   │   │   ├── syscalls-powerpc.txt
│   │   │   │   ├── syscalls-powerpc64.txt
│   │   │   │   ├── syscalls-riscv32.txt
│   │   │   │   ├── syscalls-riscv64.txt
│   │   │   │   ├── syscalls-s390.txt
│   │   │   │   ├── syscalls-s390x.txt
│   │   │   │   ├── syscalls-sparc.txt
│   │   │   │   ├── syscalls-x86_64.txt
│   │   │   │   ├── wait.h
│   │   │   │   └── xattr.h
│   │   │   └── unistd.h
│   │   └── uapi
│   │       └── linux
│   │           ├── auto_dev-ioctl.h
│   │           ├── auto_fs.h
│   │           ├── batman_adv.h
│   │           ├── bpf_common.h
│   │           ├── bpf_insn.h
│   │           ├── bpf.h
│   │           ├── btrfs_tree.h
│   │           ├── btrfs.h
│   │           ├── can
│   │           │   ├── netlink.h
│   │           │   └── vxcan.h
│   │           ├── capability.h
│   │           ├── cfm_bridge.h
│   │           ├── const.h
│   │           ├── dm-ioctl.h
│   │           ├── ethtool.h
│   │           ├── fib_rules.h
│   │           ├── filter.h
│   │           ├── fou.h
│   │           ├── fs.h
│   │           ├── fscrypt.h
│   │           ├── fsverity.h
│   │           ├── genetlink.h
│   │           ├── hdlc
│   │           │   └── ioctl.h
│   │           ├── hid.h
│   │           ├── hidraw.h
│   │           ├── if_addr.h
│   │           ├── if_addrlabel.h
│   │           ├── if_arp.h
│   │           ├── if_bonding.h
│   │           ├── if_bridge.h
│   │           ├── if_ether.h
│   │           ├── if_infiniband.h
│   │           ├── if_link.h
│   │           ├── if_macsec.h
│   │           ├── if_packet.h
│   │           ├── if_tun.h
│   │           ├── if_tunnel.h
│   │           ├── if_vlan.h
│   │           ├── if.h
│   │           ├── in.h
│   │           ├── in6.h
│   │           ├── input-event-codes.h
│   │           ├── input.h
│   │           ├── ioprio.h
│   │           ├── ip.h
│   │           ├── ip6_tunnel.h
│   │           ├── ipv6_route.h
│   │           ├── ipv6.h
│   │           ├── keyctl.h
│   │           ├── l2tp.h
│   │           ├── libc-compat.h
│   │           ├── limits.h
│   │           ├── loop.h
│   │           ├── magic.h
│   │           ├── mempolicy.h
│   │           ├── mount.h
│   │           ├── mrp_bridge.h
│   │           ├── neighbour.h
│   │           ├── net_namespace.h
│   │           ├── netdevice.h
│   │           ├── netfilter
│   │           │   ├── nf_conntrack_common.h
│   │           │   ├── nf_conntrack_tuple_common.h
│   │           │   ├── nf_nat.h
│   │           │   ├── nf_tables.h
│   │           │   ├── nfnetlink_compat.h
│   │           │   ├── nfnetlink.h
│   │           │   ├── x_tables.h
│   │           │   ├── xt_addrtype.h
│   │           │   └── xt_tcpudp.h
│   │           ├── netfilter_ipv4
│   │           │   └── ip_tables.h
│   │           ├── netfilter_ipv4.h
│   │           ├── netfilter.h
│   │           ├── netlink.h
│   │           ├── nexthop.h
│   │           ├── nl80211.h
│   │           ├── pkt_sched.h
│   │           ├── prctl.h
│   │           ├── rtnetlink.h
│   │           ├── sched
│   │           │   └── types.h
│   │           ├── socket.h
│   │           ├── sockios.h
│   │           ├── stat.h
│   │           ├── stddef.h
│   │           ├── update.sh
│   │           ├── veth.h
│   │           ├── vm_sockets.h
│   │           ├── wireguard.h
│   │           └── xattr.h
│   ├── integritysetup
│   │   ├── integrity-util.c
│   │   ├── integrity-util.h
│   │   ├── integritysetup-generator.c
│   │   ├── integritysetup.c
│   │   └── meson.build
│   ├── journal
│   │   ├── bsod.c
│   │   ├── cat.c
│   │   ├── fuzz-journald-audit.c
│   │   ├── fuzz-journald-kmsg.c
│   │   ├── fuzz-journald-native-fd.c
│   │   ├── fuzz-journald-native.c
│   │   ├── fuzz-journald-stream.c
│   │   ├── fuzz-journald-stream.options
│   │   ├── fuzz-journald-syslog.c
│   │   ├── fuzz-journald.c
│   │   ├── fuzz-journald.h
│   │   ├── journalctl-authenticate.c
│   │   ├── journalctl-authenticate.h
│   │   ├── journalctl-catalog.c
│   │   ├── journalctl-catalog.h
│   │   ├── journalctl-filter.c
│   │   ├── journalctl-filter.h
│   │   ├── journalctl-misc.c
│   │   ├── journalctl-misc.h
│   │   ├── journalctl-show.c
│   │   ├── journalctl-show.h
│   │   ├── journalctl-util.c
│   │   ├── journalctl-util.h
│   │   ├── journalctl-varlink.c
│   │   ├── journalctl-varlink.h
│   │   ├── journalctl.c
│   │   ├── journalctl.h
│   │   ├── journald-audit.c
│   │   ├── journald-audit.h
│   │   ├── journald-client.c
│   │   ├── journald-client.h
│   │   ├── journald-console.c
│   │   ├── journald-console.h
│   │   ├── journald-context.c
│   │   ├── journald-context.h
│   │   ├── journald-forward.h
│   │   ├── journald-gperf.gperf
│   │   ├── journald-kmsg.c
│   │   ├── journald-kmsg.h
│   │   ├── journald-manager.c
│   │   ├── journald-manager.h
│   │   ├── journald-native.c
│   │   ├── journald-native.h
│   │   ├── journald-rate-limit.c
│   │   ├── journald-rate-limit.h
│   │   ├── journald-socket.c
│   │   ├── journald-socket.h
│   │   ├── journald-stream.c
│   │   ├── journald-stream.h
│   │   ├── journald-sync.c
│   │   ├── journald-sync.h
│   │   ├── journald-syslog.c
│   │   ├── journald-syslog.h
│   │   ├── journald-varlink.c
│   │   ├── journald-varlink.h
│   │   ├── journald-wall.c
│   │   ├── journald-wall.h
│   │   ├── journald.c
│   │   ├── journald.conf
│   │   ├── meson.build
│   │   ├── test-journald-config.c
│   │   ├── test-journald-rate-limit.c
│   │   ├── test-journald-syslog.c
│   │   └── test-journald-tables.c
│   ├── journal-remote
│   │   ├── browse.html
│   │   ├── fuzz-journal-remote.c
│   │   ├── fuzz-journal-remote.options
│   │   ├── journal-compression-util.c
│   │   ├── journal-compression-util.h
│   │   ├── journal-gatewayd.c
│   │   ├── journal-header-util.c
│   │   ├── journal-header-util.h
│   │   ├── journal-remote-main.c
│   │   ├── journal-remote-parse.c
│   │   ├── journal-remote-parse.h
│   │   ├── journal-remote-write.c
│   │   ├── journal-remote-write.h
│   │   ├── journal-remote.c
│   │   ├── journal-remote.conf.in
│   │   ├── journal-remote.h
│   │   ├── journal-upload-journal.c
│   │   ├── journal-upload.c
│   │   ├── journal-upload.conf.in
│   │   ├── journal-upload.h
│   │   ├── log-generator.py
│   │   ├── meson.build
│   │   ├── microhttpd-util.c
│   │   ├── microhttpd-util.h
│   │   └── test-journal-header-util.c
│   ├── kernel-install
│   │   ├── 50-depmod.install
│   │   ├── 60-ukify.install.in
│   │   ├── 90-loaderentry.install.in
│   │   ├── 90-uki-copy.install
│   │   ├── install.conf
│   │   ├── kernel-install.c
│   │   ├── meson.build
│   │   ├── test-kernel-install.sh
│   │   └── uki.conf
│   ├── keyutil
│   │   ├── keyutil.c
│   │   └── meson.build
│   ├── libc
│   │   ├── bpf.c
│   │   ├── ioprio.c
│   │   ├── kcmp.c
│   │   ├── keyctl.c
│   │   ├── mempolicy.c
│   │   ├── meson.build
│   │   ├── mount.c
│   │   ├── pidfd.c
│   │   ├── quota.c
│   │   ├── sched.c
│   │   ├── signal.c
│   │   ├── stat.c
│   │   ├── unistd.c
│   │   └── xattr.c
│   ├── libsystemd
│   │   ├── libsystemd.pc.in
│   │   ├── libsystemd.sym
│   │   ├── meson.build
│   │   ├── sd-bus
│   │   │   ├── bus-common-errors.c
│   │   │   ├── bus-common-errors.h
│   │   │   ├── bus-container.c
│   │   │   ├── bus-container.h
│   │   │   ├── bus-control.c
│   │   │   ├── bus-control.h
│   │   │   ├── bus-convenience.c
│   │   │   ├── bus-creds.c
│   │   │   ├── bus-creds.h
│   │   │   ├── bus-dump-json.c
│   │   │   ├── bus-dump.c
│   │   │   ├── bus-dump.h
│   │   │   ├── bus-error.c
│   │   │   ├── bus-error.h
│   │   │   ├── bus-forward.h
│   │   │   ├── bus-internal.c
│   │   │   ├── bus-internal.h
│   │   │   ├── bus-introspect.c
│   │   │   ├── bus-introspect.h
│   │   │   ├── bus-kernel.c
│   │   │   ├── bus-kernel.h
│   │   │   ├── bus-match.c
│   │   │   ├── bus-match.h
│   │   │   ├── bus-message.c
│   │   │   ├── bus-message.h
│   │   │   ├── bus-objects.c
│   │   │   ├── bus-objects.h
│   │   │   ├── bus-protocol.h
│   │   │   ├── bus-signature.c
│   │   │   ├── bus-signature.h
│   │   │   ├── bus-slot.c
│   │   │   ├── bus-slot.h
│   │   │   ├── bus-socket.c
│   │   │   ├── bus-socket.h
│   │   │   ├── bus-track.c
│   │   │   ├── bus-track.h
│   │   │   ├── bus-type.c
│   │   │   ├── bus-type.h
│   │   │   ├── fuzz-bus-match.c
│   │   │   ├── fuzz-bus-match.options
│   │   │   ├── fuzz-bus-message.c
│   │   │   ├── sd-bus.c
│   │   │   ├── test-bus-address.c
│   │   │   ├── test-bus-benchmark.c
│   │   │   ├── test-bus-chat.c
│   │   │   ├── test-bus-cleanup.c
│   │   │   ├── test-bus-creds.c
│   │   │   ├── test-bus-error.c
│   │   │   ├── test-bus-introspect.c
│   │   │   ├── test-bus-marshal.c
│   │   │   ├── test-bus-match.c
│   │   │   ├── test-bus-objects.c
│   │   │   ├── test-bus-peersockaddr.c
│   │   │   ├── test-bus-queue-ref-cycle.c
│   │   │   ├── test-bus-server.c
│   │   │   ├── test-bus-signature.c
│   │   │   ├── test-bus-track.c
│   │   │   ├── test-bus-vtable-cc.cc -> test-bus-vtable.c
│   │   │   ├── test-bus-vtable.c
│   │   │   ├── test-bus-watch-bind.c
│   │   │   └── test-vtable-data.h
│   │   ├── sd-daemon
│   │   │   └── sd-daemon.c
│   │   ├── sd-device
│   │   │   ├── device-enumerator-private.h
│   │   │   ├── device-enumerator.c
│   │   │   ├── device-filter.c
│   │   │   ├── device-filter.h
│   │   │   ├── device-internal.h
│   │   │   ├── device-monitor-private.h
│   │   │   ├── device-monitor.c
│   │   │   ├── device-private.c
│   │   │   ├── device-private.h
│   │   │   ├── device-util.c
│   │   │   ├── device-util.h
│   │   │   ├── sd-device.c
│   │   │   ├── test-device-util.c
│   │   │   ├── test-sd-device-monitor.c
│   │   │   ├── test-sd-device-thread.c
│   │   │   └── test-sd-device.c
│   │   ├── sd-event
│   │   │   ├── event-source.h
│   │   │   ├── event-util.c
│   │   │   ├── event-util.h
│   │   │   ├── sd-event.c
│   │   │   └── test-event.c
│   │   ├── sd-hwdb
│   │   │   ├── hwdb-internal.h
│   │   │   └── sd-hwdb.c
│   │   ├── sd-id128
│   │   │   ├── id128-util.c
│   │   │   ├── id128-util.h
│   │   │   └── sd-id128.c
│   │   ├── sd-journal
│   │   │   ├── audit_type-to-name.awk
│   │   │   ├── audit-type.c
│   │   │   ├── audit-type.h
│   │   │   ├── catalog.c
│   │   │   ├── catalog.h
│   │   │   ├── fsprg.c
│   │   │   ├── fsprg.h
│   │   │   ├── generate-audit_type-list.sh
│   │   │   ├── journal-authenticate.c
│   │   │   ├── journal-authenticate.h
│   │   │   ├── journal-def.h
│   │   │   ├── journal-file.c
│   │   │   ├── journal-file.h
│   │   │   ├── journal-internal.h
│   │   │   ├── journal-send.c
│   │   │   ├── journal-send.h
│   │   │   ├── journal-vacuum.c
│   │   │   ├── journal-vacuum.h
│   │   │   ├── journal-verify.c
│   │   │   ├── journal-verify.h
│   │   │   ├── lookup3.c
│   │   │   ├── lookup3.h
│   │   │   ├── meson.build
│   │   │   ├── mmap-cache.c
│   │   │   ├── mmap-cache.h
│   │   │   ├── sd-journal.c
│   │   │   ├── test-audit-type.c
│   │   │   ├── test-catalog.c
│   │   │   ├── test-journal-append.c
│   │   │   ├── test-journal-enum.c
│   │   │   ├── test-journal-file.c
│   │   │   ├── test-journal-flush.c
│   │   │   ├── test-journal-init.c
│   │   │   ├── test-journal-interleaving.c
│   │   │   ├── test-journal-match.c
│   │   │   ├── test-journal-send.c
│   │   │   ├── test-journal-stream.c
│   │   │   ├── test-journal-verify.c
│   │   │   ├── test-journal.c
│   │   │   └── test-mmap-cache.c
│   │   ├── sd-json
│   │   │   ├── json-internal.h
│   │   │   ├── json-util.c
│   │   │   ├── json-util.h
│   │   │   └── sd-json.c
│   │   ├── sd-login
│   │   │   ├── sd-login.c
│   │   │   ├── test-login.c
│   │   │   └── test-sd-login.c
│   │   ├── sd-netlink
│   │   │   ├── netlink-genl.c
│   │   │   ├── netlink-genl.h
│   │   │   ├── netlink-internal.h
│   │   │   ├── netlink-message-nfnl.c
│   │   │   ├── netlink-message-rtnl.c
│   │   │   ├── netlink-message.c
│   │   │   ├── netlink-slot.c
│   │   │   ├── netlink-slot.h
│   │   │   ├── netlink-sock-diag.c
│   │   │   ├── netlink-sock-diag.h
│   │   │   ├── netlink-socket.c
│   │   │   ├── netlink-types-genl.c
│   │   │   ├── netlink-types-internal.h
│   │   │   ├── netlink-types-nfnl.c
│   │   │   ├── netlink-types-rtnl.c
│   │   │   ├── netlink-types-sdnl.c
│   │   │   ├── netlink-types.c
│   │   │   ├── netlink-types.h
│   │   │   ├── netlink-util.c
│   │   │   ├── netlink-util.h
│   │   │   ├── sd-netlink.c
│   │   │   └── test-netlink.c
│   │   ├── sd-network
│   │   │   ├── network-util.c
│   │   │   ├── network-util.h
│   │   │   └── sd-network.c
│   │   ├── sd-path
│   │   │   ├── path-lookup.c
│   │   │   ├── path-lookup.h
│   │   │   └── sd-path.c
│   │   ├── sd-resolve
│   │   │   ├── resolve-private.h
│   │   │   ├── sd-resolve.c
│   │   │   └── test-resolve.c
│   │   └── sd-varlink
│   │       ├── sd-varlink-idl.c
│   │       ├── sd-varlink.c
│   │       ├── varlink-idl-util.h
│   │       ├── varlink-internal.h
│   │       ├── varlink-io.systemd.c
│   │       ├── varlink-io.systemd.h
│   │       ├── varlink-org.varlink.service.c
│   │       ├── varlink-org.varlink.service.h
│   │       ├── varlink-util.c
│   │       └── varlink-util.h
│   ├── libsystemd-network
│   │   ├── arp-util.c
│   │   ├── arp-util.h
│   │   ├── dhcp-client-id-internal.h
│   │   ├── dhcp-client-internal.h
│   │   ├── dhcp-duid-internal.h
│   │   ├── dhcp-lease-internal.h
│   │   ├── dhcp-network.c
│   │   ├── dhcp-network.h
│   │   ├── dhcp-option.c
│   │   ├── dhcp-option.h
│   │   ├── dhcp-packet.c
│   │   ├── dhcp-packet.h
│   │   ├── dhcp-protocol.h
│   │   ├── dhcp-server-internal.h
│   │   ├── dhcp-server-lease-internal.h
│   │   ├── dhcp6-client-internal.h
│   │   ├── dhcp6-internal.h
│   │   ├── dhcp6-lease-internal.h
│   │   ├── dhcp6-network.c
│   │   ├── dhcp6-option.c
│   │   ├── dhcp6-option.h
│   │   ├── dhcp6-protocol.c
│   │   ├── dhcp6-protocol.h
│   │   ├── dns-resolver-internal.h
│   │   ├── fuzz-dhcp-client.c
│   │   ├── fuzz-dhcp-server-relay.c
│   │   ├── fuzz-dhcp-server.c
│   │   ├── fuzz-dhcp6-client.c
│   │   ├── fuzz-dhcp6-client.options
│   │   ├── fuzz-lldp-rx.c
│   │   ├── fuzz-lldp-rx.options
│   │   ├── fuzz-ndisc-rs.c
│   │   ├── fuzz-ndisc-rs.options
│   │   ├── icmp6-packet.c
│   │   ├── icmp6-packet.h
│   │   ├── icmp6-test-util.c
│   │   ├── icmp6-test-util.h
│   │   ├── icmp6-util.c
│   │   ├── icmp6-util.h
│   │   ├── lldp-neighbor.c
│   │   ├── lldp-neighbor.h
│   │   ├── lldp-network.c
│   │   ├── lldp-network.h
│   │   ├── lldp-rx-internal.h
│   │   ├── meson.build
│   │   ├── ndisc-internal.h
│   │   ├── ndisc-neighbor-internal.h
│   │   ├── ndisc-option.c
│   │   ├── ndisc-option.h
│   │   ├── ndisc-redirect-internal.h
│   │   ├── ndisc-router-internal.h
│   │   ├── ndisc-router-solicit-internal.h
│   │   ├── network-common.c
│   │   ├── network-common.h
│   │   ├── network-internal.c
│   │   ├── network-internal.h
│   │   ├── radv-internal.h
│   │   ├── sd-dhcp-client-id.c
│   │   ├── sd-dhcp-client.c
│   │   ├── sd-dhcp-duid.c
│   │   ├── sd-dhcp-lease.c
│   │   ├── sd-dhcp-server-lease.c
│   │   ├── sd-dhcp-server.c
│   │   ├── sd-dhcp6-client.c
│   │   ├── sd-dhcp6-lease.c
│   │   ├── sd-dns-resolver.c
│   │   ├── sd-dns-resolver.h
│   │   ├── sd-ipv4acd.c
│   │   ├── sd-ipv4ll.c
│   │   ├── sd-lldp-rx.c
│   │   ├── sd-lldp-tx.c
│   │   ├── sd-ndisc-neighbor.c
│   │   ├── sd-ndisc-redirect.c
│   │   ├── sd-ndisc-router-solicit.c
│   │   ├── sd-ndisc-router.c
│   │   ├── sd-ndisc.c
│   │   ├── sd-radv.c
│   │   ├── test-acd.c
│   │   ├── test-dhcp-client.c
│   │   ├── test-dhcp-option.c
│   │   ├── test-dhcp-server.c
│   │   ├── test-dhcp6-client.c
│   │   ├── test-ipv4ll-manual.c
│   │   ├── test-ipv4ll.c
│   │   ├── test-lldp-rx.c
│   │   ├── test-ndisc-ra.c
│   │   ├── test-ndisc-rs.c
│   │   ├── test-ndisc-send.c
│   │   └── test-sd-dhcp-lease.c
│   ├── libudev
│   │   ├── libudev-device-internal.h
│   │   ├── libudev-device.c
│   │   ├── libudev-enumerate.c
│   │   ├── libudev-hwdb.c
│   │   ├── libudev-list-internal.h
│   │   ├── libudev-list.c
│   │   ├── libudev-monitor.c
│   │   ├── libudev-queue.c
│   │   ├── libudev-util.c
│   │   ├── libudev-util.h
│   │   ├── libudev.c
│   │   ├── libudev.h
│   │   ├── libudev.pc.in
│   │   ├── libudev.sym
│   │   ├── meson.build
│   │   ├── test-libudev.c
│   │   └── test-udev-device-thread.c
│   ├── locale
│   │   ├── kbd-model-map
│   │   ├── language-fallback-map
│   │   ├── localectl.c
│   │   ├── localed-util.c
│   │   ├── localed-util.h
│   │   ├── localed.c
│   │   ├── meson.build
│   │   ├── org.freedesktop.locale1.conf
│   │   ├── org.freedesktop.locale1.policy
│   │   ├── org.freedesktop.locale1.service
│   │   ├── test-localed-util.c
│   │   ├── xkbcommon-util.c
│   │   └── xkbcommon-util.h
│   ├── login
│   │   ├── 10-systemd-logind-root-ignore-inhibitors.rules.example
│   │   ├── inhibit.c
│   │   ├── loginctl.c
│   │   ├── logind-action.c
│   │   ├── logind-action.h
│   │   ├── logind-brightness.c
│   │   ├── logind-brightness.h
│   │   ├── logind-button.c
│   │   ├── logind-button.h
│   │   ├── logind-core.c
│   │   ├── logind-dbus.c
│   │   ├── logind-dbus.h
│   │   ├── logind-device.c
│   │   ├── logind-device.h
│   │   ├── logind-forward.h
│   │   ├── logind-gperf.gperf
│   │   ├── logind-inhibit.c
│   │   ├── logind-inhibit.h
│   │   ├── logind-polkit.c
│   │   ├── logind-polkit.h
│   │   ├── logind-seat-dbus.c
│   │   ├── logind-seat-dbus.h
│   │   ├── logind-seat.c
│   │   ├── logind-seat.h
│   │   ├── logind-session-dbus.c
│   │   ├── logind-session-dbus.h
│   │   ├── logind-session-device.c
│   │   ├── logind-session-device.h
│   │   ├── logind-session.c
│   │   ├── logind-session.h
│   │   ├── logind-user-dbus.c
│   │   ├── logind-user-dbus.h
│   │   ├── logind-user.c
│   │   ├── logind-user.h
│   │   ├── logind-utmp.c
│   │   ├── logind-utmp.h
│   │   ├── logind-varlink.c
│   │   ├── logind-varlink.h
│   │   ├── logind-wall.c
│   │   ├── logind.c
│   │   ├── logind.conf.in
│   │   ├── logind.h
│   │   ├── meson.build
│   │   ├── org.freedesktop.login1.conf
│   │   ├── org.freedesktop.login1.policy
│   │   ├── org.freedesktop.login1.service
│   │   ├── pam_systemd_loadkey.c
│   │   ├── pam_systemd_loadkey.sym
│   │   ├── pam_systemd.c
│   │   ├── pam_systemd.sym
│   │   ├── sysfs-show.c
│   │   ├── sysfs-show.h
│   │   ├── systemd-user.in
│   │   ├── test-inhibit.c
│   │   ├── test-login-shared.c
│   │   ├── test-login-tables.c
│   │   ├── test-session-properties.c
│   │   └── user-runtime-dir.c
│   ├── machine
│   │   ├── image-dbus.c
│   │   ├── image-dbus.h
│   │   ├── image-varlink.c
│   │   ├── image-varlink.h
│   │   ├── image.c
│   │   ├── image.h
│   │   ├── machine-dbus.c
│   │   ├── machine-dbus.h
│   │   ├── machine-forward.h
│   │   ├── machine-varlink.c
│   │   ├── machine-varlink.h
│   │   ├── machine.c
│   │   ├── machine.h
│   │   ├── machinectl.c
│   │   ├── machined-core.c
│   │   ├── machined-dbus.c
│   │   ├── machined-varlink.c
│   │   ├── machined-varlink.h
│   │   ├── machined.c
│   │   ├── machined.h
│   │   ├── meson.build
│   │   ├── operation.c
│   │   ├── operation.h
│   │   ├── org.freedesktop.machine1.conf
│   │   ├── org.freedesktop.machine1.policy
│   │   ├── org.freedesktop.machine1.service
│   │   └── test-machine-tables.c
│   ├── machine-id-setup
│   │   ├── machine-id-setup-main.c
│   │   └── meson.build
│   ├── measure
│   │   ├── measure-tool.c
│   │   └── meson.build
│   ├── modules-load
│   │   ├── meson.build
│   │   └── modules-load.c
│   ├── mount
│   │   ├── meson.build
│   │   └── mount-tool.c
│   ├── mountfsd
│   │   ├── io.systemd.mount-file-system.policy
│   │   ├── meson.build
│   │   ├── mountfsd-manager.c
│   │   ├── mountfsd-manager.h
│   │   ├── mountfsd.c
│   │   └── mountwork.c
│   ├── network
│   │   ├── bpf
│   │   │   └── sysctl-monitor
│   │   │       ├── meson.build
│   │   │       ├── sysctl-monitor-skel.h
│   │   │       ├── sysctl-monitor.bpf.c
│   │   │       └── sysctl-write-event.h
│   │   ├── fuzz-netdev-parser.c
│   │   ├── fuzz-netdev-parser.options
│   │   ├── fuzz-network-parser.c
│   │   ├── fuzz-network-parser.options
│   │   ├── generator
│   │   │   ├── network-generator-main.c
│   │   │   ├── network-generator.c
│   │   │   ├── network-generator.h
│   │   │   └── test-network-generator.c
│   │   ├── meson.build
│   │   ├── netdev
│   │   │   ├── bareudp.c
│   │   │   ├── bareudp.h
│   │   │   ├── batadv.c
│   │   │   ├── batadv.h
│   │   │   ├── bond.c
│   │   │   ├── bond.h
│   │   │   ├── bridge.c
│   │   │   ├── bridge.h
│   │   │   ├── dummy.c
│   │   │   ├── dummy.h
│   │   │   ├── fou-tunnel.c
│   │   │   ├── fou-tunnel.h
│   │   │   ├── geneve.c
│   │   │   ├── geneve.h
│   │   │   ├── hsr.c
│   │   │   ├── hsr.h
│   │   │   ├── ifb.c
│   │   │   ├── ifb.h
│   │   │   ├── ipoib.c
│   │   │   ├── ipoib.h
│   │   │   ├── ipvlan.c
│   │   │   ├── ipvlan.h
│   │   │   ├── l2tp-tunnel.c
│   │   │   ├── l2tp-tunnel.h
│   │   │   ├── macsec.c
│   │   │   ├── macsec.h
│   │   │   ├── macvlan.c
│   │   │   ├── macvlan.h
│   │   │   ├── netdev-gperf.gperf
│   │   │   ├── netdev-util.c
│   │   │   ├── netdev-util.h
│   │   │   ├── netdev.c
│   │   │   ├── netdev.h
│   │   │   ├── nlmon.c
│   │   │   ├── nlmon.h
│   │   │   ├── tunnel.c
│   │   │   ├── tunnel.h
│   │   │   ├── tuntap.c
│   │   │   ├── tuntap.h
│   │   │   ├── vcan.c
│   │   │   ├── vcan.h
│   │   │   ├── veth.c
│   │   │   ├── veth.h
│   │   │   ├── vlan.c
│   │   │   ├── vlan.h
│   │   │   ├── vrf.c
│   │   │   ├── vrf.h
│   │   │   ├── vxcan.c
│   │   │   ├── vxcan.h
│   │   │   ├── vxlan.c
│   │   │   ├── vxlan.h
│   │   │   ├── wireguard.c
│   │   │   ├── wireguard.h
│   │   │   ├── wlan.c
│   │   │   ├── wlan.h
│   │   │   ├── xfrm.c
│   │   │   └── xfrm.h
│   │   ├── networkctl-address-label.c
│   │   ├── networkctl-address-label.h
│   │   ├── networkctl-config-file.c
│   │   ├── networkctl-config-file.h
│   │   ├── networkctl-description.c
│   │   ├── networkctl-description.h
│   │   ├── networkctl-dump-util.c
│   │   ├── networkctl-dump-util.h
│   │   ├── networkctl-journal.c
│   │   ├── networkctl-journal.h
│   │   ├── networkctl-link-info.c
│   │   ├── networkctl-link-info.h
│   │   ├── networkctl-list.c
│   │   ├── networkctl-list.h
│   │   ├── networkctl-lldp.c
│   │   ├── networkctl-lldp.h
│   │   ├── networkctl-misc.c
│   │   ├── networkctl-misc.h
│   │   ├── networkctl-status-link.c
│   │   ├── networkctl-status-link.h
│   │   ├── networkctl-status-system.c
│   │   ├── networkctl-status-system.h
│   │   ├── networkctl-util.c
│   │   ├── networkctl-util.h
│   │   ├── networkctl.c
│   │   ├── networkctl.h
│   │   ├── networkd-address-generation.c
│   │   ├── networkd-address-generation.h
│   │   ├── networkd-address-label.c
│   │   ├── networkd-address-label.h
│   │   ├── networkd-address-pool.c
│   │   ├── networkd-address-pool.h
│   │   ├── networkd-address.c
│   │   ├── networkd-address.h
│   │   ├── networkd-bridge-fdb.c
│   │   ├── networkd-bridge-fdb.h
│   │   ├── networkd-bridge-mdb.c
│   │   ├── networkd-bridge-mdb.h
│   │   ├── networkd-bridge-vlan.c
│   │   ├── networkd-bridge-vlan.h
│   │   ├── networkd-can.c
│   │   ├── networkd-can.h
│   │   ├── networkd-conf.c
│   │   ├── networkd-conf.h
│   │   ├── networkd-dhcp-common.c
│   │   ├── networkd-dhcp-common.h
│   │   ├── networkd-dhcp-prefix-delegation.c
│   │   ├── networkd-dhcp-prefix-delegation.h
│   │   ├── networkd-dhcp-server-bus.c
│   │   ├── networkd-dhcp-server-bus.h
│   │   ├── networkd-dhcp-server-static-lease.c
│   │   ├── networkd-dhcp-server-static-lease.h
│   │   ├── networkd-dhcp-server.c
│   │   ├── networkd-dhcp-server.h
│   │   ├── networkd-dhcp4-bus.c
│   │   ├── networkd-dhcp4-bus.h
│   │   ├── networkd-dhcp4.c
│   │   ├── networkd-dhcp4.h
│   │   ├── networkd-dhcp6-bus.c
│   │   ├── networkd-dhcp6-bus.h
│   │   ├── networkd-dhcp6.c
│   │   ├── networkd-dhcp6.h
│   │   ├── networkd-dns.c
│   │   ├── networkd-dns.h
│   │   ├── networkd-forward.h
│   │   ├── networkd-gperf.gperf
│   │   ├── networkd-ipv4acd.c
│   │   ├── networkd-ipv4acd.h
│   │   ├── networkd-ipv4ll.c
│   │   ├── networkd-ipv4ll.h
│   │   ├── networkd-ipv6-proxy-ndp.c
│   │   ├── networkd-ipv6-proxy-ndp.h
│   │   ├── networkd-ipv6ll.c
│   │   ├── networkd-ipv6ll.h
│   │   ├── networkd-json.c
│   │   ├── networkd-json.h
│   │   ├── networkd-link-bus.c
│   │   ├── networkd-link-bus.h
│   │   ├── networkd-link.c
│   │   ├── networkd-link.h
│   │   ├── networkd-lldp-rx.c
│   │   ├── networkd-lldp-rx.h
│   │   ├── networkd-lldp-tx.c
│   │   ├── networkd-lldp-tx.h
│   │   ├── networkd-manager-bus.c
│   │   ├── networkd-manager-bus.h
│   │   ├── networkd-manager-varlink.c
│   │   ├── networkd-manager-varlink.h
│   │   ├── networkd-manager.c
│   │   ├── networkd-manager.h
│   │   ├── networkd-ndisc.c
│   │   ├── networkd-ndisc.h
│   │   ├── networkd-neighbor.c
│   │   ├── networkd-neighbor.h
│   │   ├── networkd-netlabel.c
│   │   ├── networkd-netlabel.h
│   │   ├── networkd-network-bus.c
│   │   ├── networkd-network-bus.h
│   │   ├── networkd-network-gperf.gperf
│   │   ├── networkd-network.c
│   │   ├── networkd-network.h
│   │   ├── networkd-nexthop.c
│   │   ├── networkd-nexthop.h
│   │   ├── networkd-ntp.c
│   │   ├── networkd-ntp.h
│   │   ├── networkd-queue.c
│   │   ├── networkd-queue.h
│   │   ├── networkd-radv.c
│   │   ├── networkd-radv.h
│   │   ├── networkd-route-metric.c
│   │   ├── networkd-route-metric.h
│   │   ├── networkd-route-nexthop.c
│   │   ├── networkd-route-nexthop.h
│   │   ├── networkd-route-util.c
│   │   ├── networkd-route-util.h
│   │   ├── networkd-route.c
│   │   ├── networkd-route.h
│   │   ├── networkd-routing-policy-rule.c
│   │   ├── networkd-routing-policy-rule.h
│   │   ├── networkd-serialize.c
│   │   ├── networkd-serialize.h
│   │   ├── networkd-setlink.c
│   │   ├── networkd-setlink.h
│   │   ├── networkd-speed-meter.c
│   │   ├── networkd-speed-meter.h
│   │   ├── networkd-sriov.c
│   │   ├── networkd-sriov.h
│   │   ├── networkd-state-file.c
│   │   ├── networkd-state-file.h
│   │   ├── networkd-sysctl.c
│   │   ├── networkd-sysctl.h
│   │   ├── networkd-util.c
│   │   ├── networkd-util.h
│   │   ├── networkd-wifi.c
│   │   ├── networkd-wifi.h
│   │   ├── networkd-wiphy.c
│   │   ├── networkd-wiphy.h
│   │   ├── networkd.c
│   │   ├── networkd.conf
│   │   ├── org.freedesktop.network1.conf
│   │   ├── org.freedesktop.network1.policy
│   │   ├── org.freedesktop.network1.service
│   │   ├── systemd-networkd.pkla
│   │   ├── systemd-networkd.rules
│   │   ├── tc
│   │   │   ├── cake.c
│   │   │   ├── cake.h
│   │   │   ├── codel.c
│   │   │   ├── codel.h
│   │   │   ├── drr.c
│   │   │   ├── drr.h
│   │   │   ├── ets.c
│   │   │   ├── ets.h
│   │   │   ├── fifo.c
│   │   │   ├── fifo.h
│   │   │   ├── fq-codel.c
│   │   │   ├── fq-codel.h
│   │   │   ├── fq-pie.c
│   │   │   ├── fq-pie.h
│   │   │   ├── fq.c
│   │   │   ├── fq.h
│   │   │   ├── gred.c
│   │   │   ├── gred.h
│   │   │   ├── hhf.c
│   │   │   ├── hhf.h
│   │   │   ├── htb.c
│   │   │   ├── htb.h
│   │   │   ├── mq.c
│   │   │   ├── mq.h
│   │   │   ├── multiq.c
│   │   │   ├── multiq.h
│   │   │   ├── netem.c
│   │   │   ├── netem.h
│   │   │   ├── pie.c
│   │   │   ├── pie.h
│   │   │   ├── qdisc.c
│   │   │   ├── qdisc.h
│   │   │   ├── qfq.c
│   │   │   ├── qfq.h
│   │   │   ├── sfb.c
│   │   │   ├── sfb.h
│   │   │   ├── sfq.c
│   │   │   ├── sfq.h
│   │   │   ├── tbf.c
│   │   │   ├── tbf.h
│   │   │   ├── tc-util.c
│   │   │   ├── tc-util.h
│   │   │   ├── tc.c
│   │   │   ├── tc.h
│   │   │   ├── tclass.c
│   │   │   ├── tclass.h
│   │   │   ├── teql.c
│   │   │   └── teql.h
│   │   ├── test-network-tables.c
│   │   ├── test-network.c
│   │   ├── test-networkd-address.c
│   │   ├── test-networkd-conf.c
│   │   ├── test-networkd-util.c
│   │   └── wait-online
│   │       ├── dns-configuration.c
│   │       ├── dns-configuration.h
│   │       ├── wait-online-link.c
│   │       ├── wait-online-link.h
│   │       ├── wait-online-manager.c
│   │       ├── wait-online-manager.h
│   │       └── wait-online.c
│   ├── NOTES.md
│   ├── notify
│   │   ├── meson.build
│   │   └── notify.c
│   ├── nspawn
│   │   ├── fuzz-nspawn-oci.c
│   │   ├── fuzz-nspawn-oci.options
│   │   ├── fuzz-nspawn-settings.c
│   │   ├── fuzz-nspawn-settings.options
│   │   ├── meson.build
│   │   ├── nspawn-bind-user.c
│   │   ├── nspawn-bind-user.h
│   │   ├── nspawn-cgroup.c
│   │   ├── nspawn-cgroup.h
│   │   ├── nspawn-expose-ports.c
│   │   ├── nspawn-expose-ports.h
│   │   ├── nspawn-gperf.gperf
│   │   ├── nspawn-mount.c
│   │   ├── nspawn-mount.h
│   │   ├── nspawn-network.c
│   │   ├── nspawn-network.h
│   │   ├── nspawn-oci.c
│   │   ├── nspawn-oci.h
│   │   ├── nspawn-register.c
│   │   ├── nspawn-register.h
│   │   ├── nspawn-seccomp.c
│   │   ├── nspawn-seccomp.h
│   │   ├── nspawn-settings.c
│   │   ├── nspawn-settings.h
│   │   ├── nspawn-setuid.c
│   │   ├── nspawn-setuid.h
│   │   ├── nspawn-stub-pid1.c
│   │   ├── nspawn-stub-pid1.h
│   │   ├── nspawn.c
│   │   ├── nspawn.h
│   │   └── test-nspawn-tables.c
│   ├── nsresourced
│   │   ├── bpf
│   │   │   └── userns-restrict
│   │   │       ├── meson.build
│   │   │       ├── userns-restrict-skel.h
│   │   │       └── userns-restrict.bpf.c
│   │   ├── io.systemd.namespace-resource.policy
│   │   ├── meson.build
│   │   ├── nsresourced-manager.c
│   │   ├── nsresourced-manager.h
│   │   ├── nsresourced.c
│   │   ├── nsresourcework.c
│   │   ├── test-userns-restrict.c
│   │   ├── userns-registry.c
│   │   ├── userns-registry.h
│   │   ├── userns-restrict.c
│   │   └── userns-restrict.h
│   ├── nss-myhostname
│   │   ├── meson.build
│   │   ├── nss-myhostname.c
│   │   └── nss-myhostname.sym
│   ├── nss-mymachines
│   │   ├── meson.build
│   │   ├── nss-mymachines.c
│   │   └── nss-mymachines.sym
│   ├── nss-resolve
│   │   ├── meson.build
│   │   ├── nss-resolve.c
│   │   └── nss-resolve.sym
│   ├── nss-systemd
│   │   ├── meson.build
│   │   ├── nss-systemd.c
│   │   ├── nss-systemd.h
│   │   ├── nss-systemd.sym
│   │   ├── userdb-glue.c
│   │   └── userdb-glue.h
│   ├── oom
│   │   ├── meson.build
│   │   ├── oomctl.c
│   │   ├── oomd-conf.c
│   │   ├── oomd-conf.h
│   │   ├── oomd-manager-bus.c
│   │   ├── oomd-manager-bus.h
│   │   ├── oomd-manager.c
│   │   ├── oomd-manager.h
│   │   ├── oomd-util.c
│   │   ├── oomd-util.h
│   │   ├── oomd.c
│   │   ├── oomd.conf
│   │   ├── org.freedesktop.oom1.conf
│   │   ├── org.freedesktop.oom1.service
│   │   └── test-oomd-util.c
│   ├── path
│   │   ├── meson.build
│   │   └── path-tool.c
│   ├── pcrextend
│   │   ├── meson.build
│   │   └── pcrextend.c
│   ├── pcrlock
│   │   ├── meson.build
│   │   ├── pcrlock-firmware.c
│   │   ├── pcrlock-firmware.h
│   │   ├── pcrlock.c
│   │   └── pcrlock.d
│   │       ├── 350-action-efi-application.pcrlock
│   │       ├── 400-secureboot-separator.pcrlock.d
│   │       │   ├── 300-0x00000000.pcrlock
│   │       │   └── 600-0xffffffff.pcrlock
│   │       ├── 500-separator.pcrlock.d
│   │       │   ├── 300-0x00000000.pcrlock
│   │       │   └── 600-0xffffffff.pcrlock
│   │       ├── 700-action-efi-exit-boot-services.pcrlock.d
│   │       │   ├── 300-present.pcrlock
│   │       │   └── 600-absent.pcrlock
│   │       ├── 750-enter-initrd.pcrlock
│   │       ├── 800-leave-initrd.pcrlock
│   │       ├── 850-sysinit.pcrlock
│   │       ├── 900-ready.pcrlock
│   │       ├── 950-shutdown.pcrlock
│   │       └── 990-final.pcrlock
│   ├── portable
│   │   ├── meson.build
│   │   ├── org.freedesktop.portable1.conf
│   │   ├── org.freedesktop.portable1.policy
│   │   ├── org.freedesktop.portable1.service
│   │   ├── portable.c
│   │   ├── portable.h
│   │   ├── portablectl.c
│   │   ├── portabled-bus.c
│   │   ├── portabled-bus.h
│   │   ├── portabled-forward.h
│   │   ├── portabled-image-bus.c
│   │   ├── portabled-image-bus.h
│   │   ├── portabled-image.c
│   │   ├── portabled-image.h
│   │   ├── portabled-operation.c
│   │   ├── portabled-operation.h
│   │   ├── portabled.c
│   │   ├── portabled.h
│   │   └── profile
│   │       ├── default
│   │       │   └── service.conf
│   │       ├── nonetwork
│   │       │   └── service.conf
│   │       ├── strict
│   │       │   └── service.conf
│   │       └── trusted
│   │           └── service.conf
│   ├── pstore
│   │   ├── meson.build
│   │   ├── pstore.c
│   │   └── pstore.conf
│   ├── ptyfwd
│   │   ├── meson.build
│   │   └── ptyfwd-tool.c
│   ├── quotacheck
│   │   ├── meson.build
│   │   └── quotacheck.c
│   ├── random-seed
│   │   ├── meson.build
│   │   └── random-seed-tool.c
│   ├── rc-local-generator
│   │   ├── meson.build
│   │   └── rc-local-generator.c
│   ├── remount-fs
│   │   ├── meson.build
│   │   └── remount-fs.c
│   ├── repart
│   │   ├── definitions
│   │   │   ├── confext.repart.d
│   │   │   │   ├── 10-root.conf
│   │   │   │   ├── 20-root-verity.conf
│   │   │   │   └── 30-root-verity-sig.conf
│   │   │   ├── portable.repart.d
│   │   │   │   ├── 10-root.conf
│   │   │   │   ├── 20-root-verity.conf
│   │   │   │   └── 30-root-verity-sig.conf
│   │   │   └── sysext.repart.d
│   │   │       ├── 10-root.conf
│   │   │       ├── 20-root-verity.conf
│   │   │       └── 30-root-verity-sig.conf
│   │   ├── meson.build
│   │   └── repart.c
│   ├── reply-password
│   │   ├── meson.build
│   │   └── reply-password.c
│   ├── resolve
│   │   ├── dns_type-to-name.awk
│   │   ├── dns-type.c
│   │   ├── dns-type.h
│   │   ├── fuzz-dns-packet.c
│   │   ├── fuzz-dns-packet.options
│   │   ├── fuzz-etc-hosts.c
│   │   ├── fuzz-resource-record.c
│   │   ├── generate-dns_type-gperf.py
│   │   ├── generate-dns_type-list.sed
│   │   ├── meson.build
│   │   ├── org.freedesktop.resolve1.conf
│   │   ├── org.freedesktop.resolve1.policy
│   │   ├── org.freedesktop.resolve1.service
│   │   ├── resolv.conf
│   │   ├── resolvconf-compat.c
│   │   ├── resolvconf-compat.h
│   │   ├── resolvectl.c
│   │   ├── resolvectl.h
│   │   ├── resolved-bus.c
│   │   ├── resolved-bus.h
│   │   ├── resolved-conf.c
│   │   ├── resolved-conf.h
│   │   ├── resolved-def.h
│   │   ├── resolved-dns-answer.c
│   │   ├── resolved-dns-answer.h
│   │   ├── resolved-dns-cache.c
│   │   ├── resolved-dns-cache.h
│   │   ├── resolved-dns-delegate-bus.c
│   │   ├── resolved-dns-delegate-bus.h
│   │   ├── resolved-dns-delegate-gperf.gperf
│   │   ├── resolved-dns-delegate.c
│   │   ├── resolved-dns-delegate.h
│   │   ├── resolved-dns-dnssec.c
│   │   ├── resolved-dns-dnssec.h
│   │   ├── resolved-dns-packet.c
│   │   ├── resolved-dns-packet.h
│   │   ├── resolved-dns-query.c
│   │   ├── resolved-dns-query.h
│   │   ├── resolved-dns-question.c
│   │   ├── resolved-dns-question.h
│   │   ├── resolved-dns-rr.c
│   │   ├── resolved-dns-rr.h
│   │   ├── resolved-dns-scope.c
│   │   ├── resolved-dns-scope.h
│   │   ├── resolved-dns-search-domain.c
│   │   ├── resolved-dns-search-domain.h
│   │   ├── resolved-dns-server.c
│   │   ├── resolved-dns-server.h
│   │   ├── resolved-dns-stream.c
│   │   ├── resolved-dns-stream.h
│   │   ├── resolved-dns-stub.c
│   │   ├── resolved-dns-stub.h
│   │   ├── resolved-dns-synthesize.c
│   │   ├── resolved-dns-synthesize.h
│   │   ├── resolved-dns-transaction.c
│   │   ├── resolved-dns-transaction.h
│   │   ├── resolved-dns-trust-anchor.c
│   │   ├── resolved-dns-trust-anchor.h
│   │   ├── resolved-dns-zone.c
│   │   ├── resolved-dns-zone.h
│   │   ├── resolved-dnssd-bus.c
│   │   ├── resolved-dnssd-bus.h
│   │   ├── resolved-dnssd-gperf.gperf
│   │   ├── resolved-dnssd.c
│   │   ├── resolved-dnssd.h
│   │   ├── resolved-dnstls.c
│   │   ├── resolved-dnstls.h
│   │   ├── resolved-etc-hosts.c
│   │   ├── resolved-etc-hosts.h
│   │   ├── resolved-forward.h
│   │   ├── resolved-gperf.gperf
│   │   ├── resolved-link-bus.c
│   │   ├── resolved-link-bus.h
│   │   ├── resolved-link.c
│   │   ├── resolved-link.h
│   │   ├── resolved-llmnr.c
│   │   ├── resolved-llmnr.h
│   │   ├── resolved-manager.c
│   │   ├── resolved-manager.h
│   │   ├── resolved-mdns.c
│   │   ├── resolved-mdns.h
│   │   ├── resolved-resolv-conf.c
│   │   ├── resolved-resolv-conf.h
│   │   ├── resolved-socket-graveyard.c
│   │   ├── resolved-socket-graveyard.h
│   │   ├── resolved-timeouts.h
│   │   ├── resolved-util.c
│   │   ├── resolved-util.h
│   │   ├── resolved-varlink.c
│   │   ├── resolved-varlink.h
│   │   ├── resolved.c
│   │   ├── resolved.conf.in
│   │   ├── RFCs
│   │   ├── test-dns-answer.c
│   │   ├── test-dns-cache.c
│   │   ├── test-dns-packet-append.c
│   │   ├── test-dns-packet-extract.c
│   │   ├── test-dns-packet.c
│   │   ├── test-dns-query.c
│   │   ├── test-dns-question.c
│   │   ├── test-dns-rr.c
│   │   ├── test-dns-search-domain.c
│   │   ├── test-dns-synthesize.c
│   │   ├── test-dns-zone.c
│   │   ├── test-dnssec-complex.c
│   │   ├── test-dnssec.c
│   │   ├── test-resolve-tables.c
│   │   ├── test-resolved-dummy-server.c
│   │   ├── test-resolved-etc-hosts.c
│   │   ├── test-resolved-link.c
│   │   ├── test-resolved-packet.c
│   │   └── test-resolved-stream.c
│   ├── rfkill
│   │   ├── meson.build
│   │   └── rfkill.c
│   ├── rpm
│   │   ├── macros.systemd.in
│   │   ├── meson.build
│   │   ├── systemd-update-helper.in
│   │   ├── triggers.systemd.in
│   │   └── triggers.systemd.sh.in
│   ├── run
│   │   ├── meson.build
│   │   ├── run.c
│   │   └── systemd-run0.in
│   ├── run-generator
│   │   ├── meson.build
│   │   └── run-generator.c
│   ├── sbsign
│   │   ├── authenticode.h
│   │   ├── meson.build
│   │   └── sbsign.c
│   ├── shared
│   │   ├── acl-util.c
│   │   ├── acl-util.h
│   │   ├── acpi-fpdt.c
│   │   ├── acpi-fpdt.h
│   │   ├── apparmor-util.c
│   │   ├── apparmor-util.h
│   │   ├── ask-password-agent.c
│   │   ├── ask-password-agent.h
│   │   ├── ask-password-api.c
│   │   ├── ask-password-api.h
│   │   ├── async.c
│   │   ├── async.h
│   │   ├── barrier.c
│   │   ├── barrier.h
│   │   ├── base-filesystem.c
│   │   ├── base-filesystem.h
│   │   ├── battery-util.c
│   │   ├── battery-util.h
│   │   ├── binfmt-util.c
│   │   ├── binfmt-util.h
│   │   ├── bitmap.c
│   │   ├── bitmap.h
│   │   ├── blkid-util.c
│   │   ├── blkid-util.h
│   │   ├── blockdev-list.c
│   │   ├── blockdev-list.h
│   │   ├── blockdev-util.c
│   │   ├── blockdev-util.h
│   │   ├── bond-util.c
│   │   ├── bond-util.h
│   │   ├── boot-entry.c
│   │   ├── boot-entry.h
│   │   ├── boot-timestamps.c
│   │   ├── boot-timestamps.h
│   │   ├── bootspec.c
│   │   ├── bootspec.h
│   │   ├── bpf-compat.h
│   │   ├── bpf-dlopen.c
│   │   ├── bpf-dlopen.h
│   │   ├── bpf-link.c
│   │   ├── bpf-link.h
│   │   ├── bpf-program.c
│   │   ├── bpf-program.h
│   │   ├── bridge-util.c
│   │   ├── bridge-util.h
│   │   ├── btrfs-util.c
│   │   ├── btrfs-util.h
│   │   ├── bus-get-properties.c
│   │   ├── bus-get-properties.h
│   │   ├── bus-locator.c
│   │   ├── bus-locator.h
│   │   ├── bus-log-control-api.c
│   │   ├── bus-log-control-api.h
│   │   ├── bus-map-properties.c
│   │   ├── bus-map-properties.h
│   │   ├── bus-message-util.c
│   │   ├── bus-message-util.h
│   │   ├── bus-object.c
│   │   ├── bus-object.h
│   │   ├── bus-polkit.c
│   │   ├── bus-polkit.h
│   │   ├── bus-print-properties.c
│   │   ├── bus-print-properties.h
│   │   ├── bus-unit-procs.c
│   │   ├── bus-unit-procs.h
│   │   ├── bus-unit-util.c
│   │   ├── bus-unit-util.h
│   │   ├── bus-util.c
│   │   ├── bus-util.h
│   │   ├── bus-wait-for-jobs.c
│   │   ├── bus-wait-for-jobs.h
│   │   ├── bus-wait-for-units.c
│   │   ├── bus-wait-for-units.h
│   │   ├── calendarspec.c
│   │   ├── calendarspec.h
│   │   ├── cgroup-setup.c
│   │   ├── cgroup-setup.h
│   │   ├── cgroup-show.c
│   │   ├── cgroup-show.h
│   │   ├── chown-recursive.c
│   │   ├── chown-recursive.h
│   │   ├── clean-ipc.c
│   │   ├── clean-ipc.h
│   │   ├── clock-util.c
│   │   ├── clock-util.h
│   │   ├── color-util.c
│   │   ├── color-util.h
│   │   ├── common-signal.c
│   │   ├── common-signal.h
│   │   ├── compare-operator.c
│   │   ├── compare-operator.h
│   │   ├── condition.c
│   │   ├── condition.h
│   │   ├── conf-parser-forward.h
│   │   ├── conf-parser.c
│   │   ├── conf-parser.h
│   │   ├── copy.c
│   │   ├── copy.h
│   │   ├── coredump-util.c
│   │   ├── coredump-util.h
│   │   ├── cpu-set-util.c
│   │   ├── cpu-set-util.h
│   │   ├── creds-util.c
│   │   ├── creds-util.h
│   │   ├── cryptsetup-fido2.c
│   │   ├── cryptsetup-fido2.h
│   │   ├── cryptsetup-tpm2.c
│   │   ├── cryptsetup-tpm2.h
│   │   ├── cryptsetup-util.c
│   │   ├── cryptsetup-util.h
│   │   ├── daemon-util.c
│   │   ├── daemon-util.h
│   │   ├── data-fd-util.c
│   │   ├── data-fd-util.h
│   │   ├── dev-setup.c
│   │   ├── dev-setup.h
│   │   ├── device-nodes.c
│   │   ├── device-nodes.h
│   │   ├── discover-image.c
│   │   ├── discover-image.h
│   │   ├── dissect-image.c
│   │   ├── dissect-image.h
│   │   ├── dm-util.c
│   │   ├── dm-util.h
│   │   ├── dns-domain.c
│   │   ├── dns-domain.h
│   │   ├── dropin.c
│   │   ├── dropin.h
│   │   ├── edit-util.c
│   │   ├── edit-util.h
│   │   ├── efi-api.c
│   │   ├── efi-api.h
│   │   ├── efi-loader.c
│   │   ├── efi-loader.h
│   │   ├── elf-util.c
│   │   ├── elf-util.h
│   │   ├── enable-mempool.c
│   │   ├── env-file-label.c
│   │   ├── ethtool-link-mode.py
│   │   ├── ethtool-util.c
│   │   ├── ethtool-util.h
│   │   ├── exec-util.c
│   │   ├── exec-util.h
│   │   ├── exit-status.c
│   │   ├── exit-status.h
│   │   ├── extension-util.c
│   │   ├── extension-util.h
│   │   ├── factory-reset.c
│   │   ├── factory-reset.h
│   │   ├── fdisk-util.c
│   │   ├── fdisk-util.h
│   │   ├── fdset.c
│   │   ├── fdset.h
│   │   ├── fido2-util.c
│   │   ├── fido2-util.h
│   │   ├── find-esp.c
│   │   ├── find-esp.h
│   │   ├── firewall-util-iptables.c
│   │   ├── firewall-util-nft.c
│   │   ├── firewall-util-private.h
│   │   ├── firewall-util.c
│   │   ├── firewall-util.h
│   │   ├── fork-notify.c
│   │   ├── fork-notify.h
│   │   ├── format-table.c
│   │   ├── format-table.h
│   │   ├── fsck-util.h
│   │   ├── fstab-util.c
│   │   ├── fstab-util.h
│   │   ├── generate-ip-protocol-list.sh
│   │   ├── generate-syscall-list.py
│   │   ├── generator.c
│   │   ├── generator.h
│   │   ├── geneve-util.c
│   │   ├── geneve-util.h
│   │   ├── gpt.c
│   │   ├── gpt.h
│   │   ├── group-record.c
│   │   ├── group-record.h
│   │   ├── hibernate-util.c
│   │   ├── hibernate-util.h
│   │   ├── hostname-setup.c
│   │   ├── hostname-setup.h
│   │   ├── hwdb-util.c
│   │   ├── hwdb-util.h
│   │   ├── id128-print.c
│   │   ├── id128-print.h
│   │   ├── idn-util.c
│   │   ├── idn-util.h
│   │   ├── ima-util.c
│   │   ├── ima-util.h
│   │   ├── image-policy.c
│   │   ├── image-policy.h
│   │   ├── import-util.c
│   │   ├── import-util.h
│   │   ├── in-addr-prefix-util.c
│   │   ├── in-addr-prefix-util.h
│   │   ├── install-file.c
│   │   ├── install-file.h
│   │   ├── install-printf.c
│   │   ├── install-printf.h
│   │   ├── install.c
│   │   ├── install.h
│   │   ├── ioprio-util.c
│   │   ├── ioprio-util.h
│   │   ├── ip-protocol-list.c
│   │   ├── ip-protocol-list.h
│   │   ├── ip-protocol-to-name.awk
│   │   ├── ipvlan-util.c
│   │   ├── ipvlan-util.h
│   │   ├── journal-file-util.c
│   │   ├── journal-file-util.h
│   │   ├── journal-importer.c
│   │   ├── journal-importer.h
│   │   ├── journal-util.c
│   │   ├── journal-util.h
│   │   ├── kbd-util.c
│   │   ├── kbd-util.h
│   │   ├── kernel-config.c
│   │   ├── kernel-config.h
│   │   ├── kernel-image.c
│   │   ├── kernel-image.h
│   │   ├── killall.c
│   │   ├── killall.h
│   │   ├── label-util.c
│   │   ├── label-util.h
│   │   ├── libarchive-util.c
│   │   ├── libarchive-util.h
│   │   ├── libaudit-util.c
│   │   ├── libaudit-util.h
│   │   ├── libcrypt-util.c
│   │   ├── libcrypt-util.h
│   │   ├── libfido2-util.c
│   │   ├── libfido2-util.h
│   │   ├── libmount-util.c
│   │   ├── libmount-util.h
│   │   ├── libshared.sym
│   │   ├── local-addresses.c
│   │   ├── local-addresses.h
│   │   ├── locale-setup.c
│   │   ├── locale-setup.h
│   │   ├── log-link.h
│   │   ├── logs-show.c
│   │   ├── logs-show.h
│   │   ├── loop-util.c
│   │   ├── loop-util.h
│   │   ├── loopback-setup.c
│   │   ├── loopback-setup.h
│   │   ├── lsm-util.c
│   │   ├── lsm-util.h
│   │   ├── machine-bind-user.c
│   │   ├── machine-bind-user.h
│   │   ├── machine-credential.c
│   │   ├── machine-credential.h
│   │   ├── machine-id-setup.c
│   │   ├── machine-id-setup.h
│   │   ├── machine-pool.c
│   │   ├── machine-pool.h
│   │   ├── macvlan-util.c
│   │   ├── macvlan-util.h
│   │   ├── main-func.c
│   │   ├── main-func.h
│   │   ├── meson.build
│   │   ├── mkdir-label.c
│   │   ├── mkdir-label.h
│   │   ├── mkfs-util.c
│   │   ├── mkfs-util.h
│   │   ├── module-util.c
│   │   ├── module-util.h
│   │   ├── mount-setup.c
│   │   ├── mount-setup.h
│   │   ├── mount-util.c
│   │   ├── mount-util.h
│   │   ├── net-condition.c
│   │   ├── net-condition.h
│   │   ├── netif-naming-scheme.c
│   │   ├── netif-naming-scheme.h
│   │   ├── netif-sriov.c
│   │   ├── netif-sriov.h
│   │   ├── netif-util.c
│   │   ├── netif-util.h
│   │   ├── notify-recv.c
│   │   ├── notify-recv.h
│   │   ├── nsflags.c
│   │   ├── nsflags.h
│   │   ├── nsresource.c
│   │   ├── nsresource.h
│   │   ├── numa-util.c
│   │   ├── numa-util.h
│   │   ├── open-file.c
│   │   ├── open-file.h
│   │   ├── openssl-util.c
│   │   ├── openssl-util.h
│   │   ├── osc-context.c
│   │   ├── osc-context.h
│   │   ├── output-mode.c
│   │   ├── output-mode.h
│   │   ├── pager.c
│   │   ├── pager.h
│   │   ├── pam-util.c
│   │   ├── pam-util.h
│   │   ├── parse-argument.c
│   │   ├── parse-argument.h
│   │   ├── parse-helpers.c
│   │   ├── parse-helpers.h
│   │   ├── password-quality-util-passwdqc.c
│   │   ├── password-quality-util-passwdqc.h
│   │   ├── password-quality-util-pwquality.c
│   │   ├── password-quality-util-pwquality.h
│   │   ├── password-quality-util.h
│   │   ├── pcre2-util.c
│   │   ├── pcre2-util.h
│   │   ├── pcrextend-util.c
│   │   ├── pcrextend-util.h
│   │   ├── pe-binary.c
│   │   ├── pe-binary.h
│   │   ├── pkcs11-util.c
│   │   ├── pkcs11-util.h
│   │   ├── plymouth-util.c
│   │   ├── plymouth-util.h
│   │   ├── polkit-agent.c
│   │   ├── polkit-agent.h
│   │   ├── portable-util.c
│   │   ├── portable-util.h
│   │   ├── pretty-print.c
│   │   ├── pretty-print.h
│   │   ├── ptyfwd.c
│   │   ├── ptyfwd.h
│   │   ├── qrcode-util.c
│   │   ├── qrcode-util.h
│   │   ├── quota-util.c
│   │   ├── quota-util.h
│   │   ├── reboot-util.c
│   │   ├── reboot-util.h
│   │   ├── recovery-key.c
│   │   ├── recovery-key.h
│   │   ├── resize-fs.c
│   │   ├── resize-fs.h
│   │   ├── resolve-util.c
│   │   ├── resolve-util.h
│   │   ├── rm-rf.c
│   │   ├── rm-rf.h
│   │   ├── seccomp-util.c
│   │   ├── seccomp-util.h
│   │   ├── securebits-util.c
│   │   ├── securebits-util.h
│   │   ├── selinux-util.c
│   │   ├── selinux-util.h
│   │   ├── serialize.c
│   │   ├── serialize.h
│   │   ├── service-util.c
│   │   ├── service-util.h
│   │   ├── shift-uid.c
│   │   ├── shift-uid.h
│   │   ├── sleep-config.c
│   │   ├── sleep-config.h
│   │   ├── smack-util.c
│   │   ├── smack-util.h
│   │   ├── smbios11.c
│   │   ├── smbios11.h
│   │   ├── socket-label.c
│   │   ├── socket-netlink.c
│   │   ├── socket-netlink.h
│   │   ├── specifier.c
│   │   ├── specifier.h
│   │   ├── switch-root.c
│   │   ├── switch-root.h
│   │   ├── test-tables.h
│   │   ├── tests.c
│   │   ├── tests.h
│   │   ├── tmpfile-util-label.c
│   │   ├── tmpfile-util-label.h
│   │   ├── tomoyo-util.c
│   │   ├── tomoyo-util.h
│   │   ├── tpm2-event-log.c
│   │   ├── tpm2-event-log.h
│   │   ├── tpm2-util.c
│   │   ├── tpm2-util.h
│   │   ├── udev-util.c
│   │   ├── udev-util.h
│   │   ├── unit-file.c
│   │   ├── unit-file.h
│   │   ├── user-record-nss.c
│   │   ├── user-record-nss.h
│   │   ├── user-record-show.c
│   │   ├── user-record-show.h
│   │   ├── user-record.c
│   │   ├── user-record.h
│   │   ├── userdb-dropin.c
│   │   ├── userdb-dropin.h
│   │   ├── userdb.c
│   │   ├── userdb.h
│   │   ├── utmp-wtmp.c
│   │   ├── utmp-wtmp.h
│   │   ├── varlink-idl-common.c
│   │   ├── varlink-idl-common.h
│   │   ├── varlink-io.systemd.AskPassword.c
│   │   ├── varlink-io.systemd.AskPassword.h
│   │   ├── varlink-io.systemd.BootControl.c
│   │   ├── varlink-io.systemd.BootControl.h
│   │   ├── varlink-io.systemd.Credentials.c
│   │   ├── varlink-io.systemd.Credentials.h
│   │   ├── varlink-io.systemd.FactoryReset.c
│   │   ├── varlink-io.systemd.FactoryReset.h
│   │   ├── varlink-io.systemd.Hostname.c
│   │   ├── varlink-io.systemd.Hostname.h
│   │   ├── varlink-io.systemd.Import.c
│   │   ├── varlink-io.systemd.Import.h
│   │   ├── varlink-io.systemd.Journal.c
│   │   ├── varlink-io.systemd.Journal.h
│   │   ├── varlink-io.systemd.Login.c
│   │   ├── varlink-io.systemd.Login.h
│   │   ├── varlink-io.systemd.Machine.c
│   │   ├── varlink-io.systemd.Machine.h
│   │   ├── varlink-io.systemd.MachineImage.c
│   │   ├── varlink-io.systemd.MachineImage.h
│   │   ├── varlink-io.systemd.ManagedOOM.c
│   │   ├── varlink-io.systemd.ManagedOOM.h
│   │   ├── varlink-io.systemd.Manager.c
│   │   ├── varlink-io.systemd.Manager.h
│   │   ├── varlink-io.systemd.MountFileSystem.c
│   │   ├── varlink-io.systemd.MountFileSystem.h
│   │   ├── varlink-io.systemd.NamespaceResource.c
│   │   ├── varlink-io.systemd.NamespaceResource.h
│   │   ├── varlink-io.systemd.Network.c
│   │   ├── varlink-io.systemd.Network.h
│   │   ├── varlink-io.systemd.oom.c
│   │   ├── varlink-io.systemd.oom.h
│   │   ├── varlink-io.systemd.PCRExtend.c
│   │   ├── varlink-io.systemd.PCRExtend.h
│   │   ├── varlink-io.systemd.PCRLock.c
│   │   ├── varlink-io.systemd.PCRLock.h
│   │   ├── varlink-io.systemd.Resolve.c
│   │   ├── varlink-io.systemd.Resolve.h
│   │   ├── varlink-io.systemd.Resolve.Monitor.c
│   │   ├── varlink-io.systemd.Resolve.Monitor.h
│   │   ├── varlink-io.systemd.service.c
│   │   ├── varlink-io.systemd.service.h
│   │   ├── varlink-io.systemd.sysext.c
│   │   ├── varlink-io.systemd.sysext.h
│   │   ├── varlink-io.systemd.Udev.c
│   │   ├── varlink-io.systemd.Udev.h
│   │   ├── varlink-io.systemd.Unit.c
│   │   ├── varlink-io.systemd.Unit.h
│   │   ├── varlink-io.systemd.UserDatabase.c
│   │   ├── varlink-io.systemd.UserDatabase.h
│   │   ├── varlink-serialize.c
│   │   ├── varlink-serialize.h
│   │   ├── vconsole-util.c
│   │   ├── vconsole-util.h
│   │   ├── verb-log-control.c
│   │   ├── verb-log-control.h
│   │   ├── verbs.c
│   │   ├── verbs.h
│   │   ├── vlan-util.c
│   │   ├── vlan-util.h
│   │   ├── volatile-util.c
│   │   ├── volatile-util.h
│   │   ├── vpick.c
│   │   ├── vpick.h
│   │   ├── wall.c
│   │   ├── wall.h
│   │   ├── watchdog.c
│   │   ├── watchdog.h
│   │   ├── web-util.c
│   │   ├── web-util.h
│   │   ├── wifi-util.c
│   │   ├── wifi-util.h
│   │   ├── xml.c
│   │   └── xml.h
│   ├── shutdown
│   │   ├── detach-dm.c
│   │   ├── detach-dm.h
│   │   ├── detach-loopback.c
│   │   ├── detach-loopback.h
│   │   ├── detach-md.c
│   │   ├── detach-md.h
│   │   ├── detach-swap.c
│   │   ├── detach-swap.h
│   │   ├── meson.build
│   │   ├── shutdown.c
│   │   ├── shutdown.h
│   │   ├── test-umount.c
│   │   ├── umount.c
│   │   └── umount.h
│   ├── sleep
│   │   ├── battery-capacity.c
│   │   ├── battery-capacity.h
│   │   ├── meson.build
│   │   ├── sleep.c
│   │   ├── sleep.conf
│   │   └── test-battery-capacity.c
│   ├── socket-activate
│   │   ├── meson.build
│   │   └── socket-activate.c
│   ├── socket-proxy
│   │   ├── meson.build
│   │   └── socket-proxyd.c
│   ├── ssh-generator
│   │   ├── 20-systemd-ssh-proxy.conf.in
│   │   ├── meson.build
│   │   ├── ssh-generator.c
│   │   ├── ssh-issue.c
│   │   └── ssh-proxy.c
│   ├── stdio-bridge
│   │   ├── meson.build
│   │   └── stdio-bridge.c
│   ├── storagetm
│   │   ├── meson.build
│   │   └── storagetm.c
│   ├── sulogin-shell
│   │   ├── meson.build
│   │   └── sulogin-shell.c
│   ├── sysctl
│   │   ├── meson.build
│   │   └── sysctl.c
│   ├── sysext
│   │   ├── meson.build
│   │   └── sysext.c
│   ├── system-update-generator
│   │   ├── meson.build
│   │   └── system-update-generator.c
│   ├── systemctl
│   │   ├── fuzz-systemctl-parse-argv.c
│   │   ├── meson.build
│   │   ├── systemctl-add-dependency.c
│   │   ├── systemctl-add-dependency.h
│   │   ├── systemctl-cancel-job.c
│   │   ├── systemctl-cancel-job.h
│   │   ├── systemctl-clean-or-freeze.c
│   │   ├── systemctl-clean-or-freeze.h
│   │   ├── systemctl-compat-halt.c
│   │   ├── systemctl-compat-halt.h
│   │   ├── systemctl-compat-shutdown.c
│   │   ├── systemctl-compat-shutdown.h
│   │   ├── systemctl-daemon-reload.c
│   │   ├── systemctl-daemon-reload.h
│   │   ├── systemctl-edit.c
│   │   ├── systemctl-edit.h
│   │   ├── systemctl-enable.c
│   │   ├── systemctl-enable.h
│   │   ├── systemctl-is-active.c
│   │   ├── systemctl-is-active.h
│   │   ├── systemctl-is-enabled.c
│   │   ├── systemctl-is-enabled.h
│   │   ├── systemctl-is-system-running.c
│   │   ├── systemctl-is-system-running.h
│   │   ├── systemctl-kill.c
│   │   ├── systemctl-kill.h
│   │   ├── systemctl-list-dependencies.c
│   │   ├── systemctl-list-dependencies.h
│   │   ├── systemctl-list-jobs.c
│   │   ├── systemctl-list-jobs.h
│   │   ├── systemctl-list-machines.c
│   │   ├── systemctl-list-machines.h
│   │   ├── systemctl-list-unit-files.c
│   │   ├── systemctl-list-unit-files.h
│   │   ├── systemctl-list-units.c
│   │   ├── systemctl-list-units.h
│   │   ├── systemctl-log-setting.c
│   │   ├── systemctl-log-setting.h
│   │   ├── systemctl-logind.c
│   │   ├── systemctl-logind.h
│   │   ├── systemctl-main.c
│   │   ├── systemctl-mount.c
│   │   ├── systemctl-mount.h
│   │   ├── systemctl-preset-all.c
│   │   ├── systemctl-preset-all.h
│   │   ├── systemctl-reset-failed.c
│   │   ├── systemctl-reset-failed.h
│   │   ├── systemctl-service-watchdogs.c
│   │   ├── systemctl-service-watchdogs.h
│   │   ├── systemctl-set-default.c
│   │   ├── systemctl-set-default.h
│   │   ├── systemctl-set-environment.c
│   │   ├── systemctl-set-environment.h
│   │   ├── systemctl-set-property.c
│   │   ├── systemctl-set-property.h
│   │   ├── systemctl-show.c
│   │   ├── systemctl-show.h
│   │   ├── systemctl-start-special.c
│   │   ├── systemctl-start-special.h
│   │   ├── systemctl-start-unit.c
│   │   ├── systemctl-start-unit.h
│   │   ├── systemctl-switch-root.c
│   │   ├── systemctl-switch-root.h
│   │   ├── systemctl-sysv-compat.c
│   │   ├── systemctl-sysv-compat.h
│   │   ├── systemctl-trivial-method.c
│   │   ├── systemctl-trivial-method.h
│   │   ├── systemctl-util.c
│   │   ├── systemctl-util.h
│   │   ├── systemctl-whoami.c
│   │   ├── systemctl-whoami.h
│   │   ├── systemctl.c
│   │   ├── systemctl.h
│   │   └── systemd-sysv-install.SKELETON
│   ├── systemd
│   │   ├── _sd-common.h
│   │   ├── meson.build
│   │   ├── sd-bus-protocol.h
│   │   ├── sd-bus-vtable.h
│   │   ├── sd-bus.h
│   │   ├── sd-daemon.h
│   │   ├── sd-device.h
│   │   ├── sd-dhcp-client-id.h
│   │   ├── sd-dhcp-client.h
│   │   ├── sd-dhcp-duid.h
│   │   ├── sd-dhcp-lease.h
│   │   ├── sd-dhcp-option.h
│   │   ├── sd-dhcp-protocol.h
│   │   ├── sd-dhcp-server-lease.h
│   │   ├── sd-dhcp-server.h
│   │   ├── sd-dhcp6-client.h
│   │   ├── sd-dhcp6-lease.h
│   │   ├── sd-dhcp6-option.h
│   │   ├── sd-dhcp6-protocol.h
│   │   ├── sd-event.h
│   │   ├── sd-gpt.h
│   │   ├── sd-hwdb.h
│   │   ├── sd-id128.h
│   │   ├── sd-ipv4acd.h
│   │   ├── sd-ipv4ll.h
│   │   ├── sd-journal.h
│   │   ├── sd-json.h
│   │   ├── sd-lldp-rx.h
│   │   ├── sd-lldp-tx.h
│   │   ├── sd-lldp.h
│   │   ├── sd-login.h
│   │   ├── sd-messages.h
│   │   ├── sd-ndisc-neighbor.h
│   │   ├── sd-ndisc-protocol.h
│   │   ├── sd-ndisc-redirect.h
│   │   ├── sd-ndisc-router-solicit.h
│   │   ├── sd-ndisc-router.h
│   │   ├── sd-ndisc.h
│   │   ├── sd-netlink.h
│   │   ├── sd-network.h
│   │   ├── sd-path.h
│   │   ├── sd-radv.h
│   │   ├── sd-resolve.h
│   │   ├── sd-utf8.h
│   │   ├── sd-varlink-idl.h
│   │   └── sd-varlink.h
│   ├── sysupdate
│   │   ├── meson.build
│   │   ├── org.freedesktop.sysupdate1.conf
│   │   ├── org.freedesktop.sysupdate1.policy
│   │   ├── org.freedesktop.sysupdate1.service
│   │   ├── sysupdate-cache.c
│   │   ├── sysupdate-cache.h
│   │   ├── sysupdate-feature.c
│   │   ├── sysupdate-feature.h
│   │   ├── sysupdate-forward.h
│   │   ├── sysupdate-instance.c
│   │   ├── sysupdate-instance.h
│   │   ├── sysupdate-partition.c
│   │   ├── sysupdate-partition.h
│   │   ├── sysupdate-pattern.c
│   │   ├── sysupdate-pattern.h
│   │   ├── sysupdate-resource.c
│   │   ├── sysupdate-resource.h
│   │   ├── sysupdate-transfer.c
│   │   ├── sysupdate-transfer.h
│   │   ├── sysupdate-update-set-flags.c
│   │   ├── sysupdate-update-set-flags.h
│   │   ├── sysupdate-update-set.c
│   │   ├── sysupdate-update-set.h
│   │   ├── sysupdate-util.c
│   │   ├── sysupdate-util.h
│   │   ├── sysupdate.c
│   │   ├── sysupdate.h
│   │   ├── sysupdated.c
│   │   └── updatectl.c
│   ├── sysusers
│   │   ├── meson.build
│   │   └── sysusers.c
│   ├── sysv-generator
│   │   ├── meson.build
│   │   └── sysv-generator.c
│   ├── test
│   │   ├── generate-sym-test.py
│   │   ├── meson.build
│   │   ├── nss-test-util.c
│   │   ├── nss-test-util.h
│   │   ├── test-acl-util.c
│   │   ├── test-af-list.c
│   │   ├── test-alloc-util.c
│   │   ├── test-architecture.c
│   │   ├── test-argv-util.c
│   │   ├── test-arphrd-util.c
│   │   ├── test-ask-password-api.c
│   │   ├── test-async.c
│   │   ├── test-audit-util.c
│   │   ├── test-barrier.c
│   │   ├── test-binfmt-util.c
│   │   ├── test-bitfield.c
│   │   ├── test-bitmap.c
│   │   ├── test-blockdev-util.c
│   │   ├── test-boot-timestamps.c
│   │   ├── test-bootspec.c
│   │   ├── test-bpf-devices.c
│   │   ├── test-bpf-firewall.c
│   │   ├── test-bpf-foreign-programs.c
│   │   ├── test-bpf-restrict-fs.c
│   │   ├── test-bpf-token.c
│   │   ├── test-btrfs-physical-offset.c
│   │   ├── test-btrfs.c
│   │   ├── test-build-path.c
│   │   ├── test-bus-unit-util.c
│   │   ├── test-bus-util.c
│   │   ├── test-calendarspec.c
│   │   ├── test-capability-list.c
│   │   ├── test-capability-util.c
│   │   ├── test-cgroup-cpu.c
│   │   ├── test-cgroup-mask.c
│   │   ├── test-cgroup-unit-default.c
│   │   ├── test-cgroup-util.c
│   │   ├── test-cgroup.c
│   │   ├── test-chase-manual.c
│   │   ├── test-chase.c
│   │   ├── test-chid.c
│   │   ├── test-chown-rec.c
│   │   ├── test-clock.c
│   │   ├── test-color-util.c
│   │   ├── test-compare-operator.c
│   │   ├── test-compress-benchmark.c
│   │   ├── test-compress.c
│   │   ├── test-condition.c
│   │   ├── test-conf-files.c
│   │   ├── test-conf-parser.c
│   │   ├── test-copy.c
│   │   ├── test-core-unit.c
│   │   ├── test-coredump-util.c
│   │   ├── test-cpu-set-util.c
│   │   ├── test-creds.c
│   │   ├── test-cryptolib.c
│   │   ├── test-daemon.c
│   │   ├── test-data-fd-util.c
│   │   ├── test-date.c
│   │   ├── test-dev-setup.c
│   │   ├── test-device-nodes.c
│   │   ├── test-devnum-util.c
│   │   ├── test-dirent-util.c
│   │   ├── test-display-quota.c
│   │   ├── test-dlopen-so.c
│   │   ├── test-dlopen.c
│   │   ├── test-dns-domain.c
│   │   ├── test-ellipsize.c
│   │   ├── test-emergency-action.c
│   │   ├── test-engine.c
│   │   ├── test-env-file.c
│   │   ├── test-env-util.c
│   │   ├── test-errno-list.c
│   │   ├── test-errno-util.c
│   │   ├── test-escape.c
│   │   ├── test-ether-addr-util.c
│   │   ├── test-exec-util.c
│   │   ├── test-execute.c
│   │   ├── test-execve.c
│   │   ├── test-exit-status.c
│   │   ├── test-extract-word.c
│   │   ├── test-fd-util.c
│   │   ├── test-fdset.c
│   │   ├── test-fiemap.c
│   │   ├── test-fileio.c
│   │   ├── test-firewall-util.c
│   │   ├── test-format-table.c
│   │   ├── test-format-util.c
│   │   ├── test-fs-util.c
│   │   ├── test-fstab-util.c
│   │   ├── test-glob-util.c
│   │   ├── test-gpt.c
│   │   ├── test-gunicode.c
│   │   ├── test-hash-funcs.c
│   │   ├── test-hashmap-ordered.awk
│   │   ├── test-hashmap-plain.c
│   │   ├── test-hashmap.c
│   │   ├── test-hexdecoct.c
│   │   ├── test-hmac.c
│   │   ├── test-hostname-setup.c
│   │   ├── test-hostname-util.c
│   │   ├── test-id128.c
│   │   ├── test-image-filter.c
│   │   ├── test-image-policy.c
│   │   ├── test-import-util.c
│   │   ├── test-in-addr-prefix-util.c
│   │   ├── test-in-addr-util.c
│   │   ├── test-install-file.c
│   │   ├── test-install-root.c
│   │   ├── test-install.c
│   │   ├── test-io-util.c
│   │   ├── test-iovec-util.c
│   │   ├── test-ip-protocol-list.c
│   │   ├── test-ipcrm.c
│   │   ├── test-job-type.c
│   │   ├── test-journal-importer.c
│   │   ├── test-json.c
│   │   ├── test-kbd-util.c
│   │   ├── test-label.c
│   │   ├── test-libcrypt-util.c
│   │   ├── test-libmount.c
│   │   ├── test-limits-util.c
│   │   ├── test-list.c
│   │   ├── test-load-fragment.c
│   │   ├── test-local-addresses.c
│   │   ├── test-locale-util.c
│   │   ├── test-lock-util.c
│   │   ├── test-log.c
│   │   ├── test-logarithm.c
│   │   ├── test-login-util.c
│   │   ├── test-loop-block.c
│   │   ├── test-loopback.c
│   │   ├── test-macro.c
│   │   ├── test-math-util.c
│   │   ├── test-memfd-util.c
│   │   ├── test-memory-util.c
│   │   ├── test-mempool.c
│   │   ├── test-mempress.c
│   │   ├── test-memstream-util.c
│   │   ├── test-mkdir.c
│   │   ├── test-modhex.c
│   │   ├── test-mount-util.c
│   │   ├── test-mountpoint-util.c
│   │   ├── test-namespace.c
│   │   ├── test-net-naming-scheme.c
│   │   ├── test-netlink-manual.c
│   │   ├── test-nft-set.c
│   │   ├── test-notify-recv.c
│   │   ├── test-ns.c
│   │   ├── test-nsresource.c
│   │   ├── test-nss-hosts.c
│   │   ├── test-nss-users.c
│   │   ├── test-nulstr-util.c
│   │   ├── test-open-file.c
│   │   ├── test-openssl.c
│   │   ├── test-ordered-set.c
│   │   ├── test-os-util.c
│   │   ├── test-osc-context.c
│   │   ├── test-parse-argument.c
│   │   ├── test-parse-helpers.c
│   │   ├── test-parse-util.c
│   │   ├── test-path-lookup.c
│   │   ├── test-path-util.c
│   │   ├── test-path.c
│   │   ├── test-percent-util.c
│   │   ├── test-pidref.c
│   │   ├── test-pretty-print.c
│   │   ├── test-prioq.c
│   │   ├── test-proc-cmdline.c
│   │   ├── test-process-util.c
│   │   ├── test-procfs-util.c
│   │   ├── test-progress-bar.c
│   │   ├── test-psi-util.c
│   │   ├── test-qrcode-util.c
│   │   ├── test-random-util.c
│   │   ├── test-ratelimit.c
│   │   ├── test-raw-clone.c
│   │   ├── test-recovery-key.c
│   │   ├── test-recurse-dir.c
│   │   ├── test-replace-var.c
│   │   ├── test-rlimit-util.c
│   │   ├── test-rm-rf.c
│   │   ├── test-sbat.c
│   │   ├── test-sched-prio.c
│   │   ├── test-sd-hwdb.c
│   │   ├── test-sd-path.c
│   │   ├── test-seccomp.c
│   │   ├── test-secure-bits.c
│   │   ├── test-selinux.c
│   │   ├── test-serialize.c
│   │   ├── test-set-disable-mempool.c
│   │   ├── test-set.c
│   │   ├── test-sha1.c
│   │   ├── test-sha256.c
│   │   ├── test-shift-uid.c
│   │   ├── test-sigbus.c
│   │   ├── test-signal-util.c
│   │   ├── test-siphash24.c
│   │   ├── test-sizeof.c
│   │   ├── test-sleep-config.c
│   │   ├── test-socket-bind.c
│   │   ├── test-socket-netlink.c
│   │   ├── test-socket-util.c
│   │   ├── test-specifier.c
│   │   ├── test-stat-util.c
│   │   ├── test-static-destruct.c
│   │   ├── test-strbuf.c
│   │   ├── test-string-util.c
│   │   ├── test-strip-tab-ansi.c
│   │   ├── test-strv.c
│   │   ├── test-strxcpyx.c
│   │   ├── test-sysctl-util.c
│   │   ├── test-tables.c
│   │   ├── test-taint.c
│   │   ├── test-terminal-util.c
│   │   ├── test-tests.c
│   │   ├── test-time-util.c
│   │   ├── test-tmpfile-util.c
│   │   ├── test-tpm2.c
│   │   ├── test-udev-util.c
│   │   ├── test-uid-classification.c
│   │   ├── test-uid-range.c
│   │   ├── test-umask-util.c
│   │   ├── test-unaligned.c
│   │   ├── test-unit-file.c
│   │   ├── test-unit-name.c
│   │   ├── test-unit-serialize.c
│   │   ├── test-user-record.c
│   │   ├── test-user-util.c
│   │   ├── test-utf8.c
│   │   ├── test-utmp.c
│   │   ├── test-varlink-idl.c
│   │   ├── test-varlink.c
│   │   ├── test-verbs.c
│   │   ├── test-vpick.c
│   │   ├── test-watch-pid.c
│   │   ├── test-watchdog.c
│   │   ├── test-web-util.c
│   │   ├── test-xattr-util.c
│   │   └── test-xml.c
│   ├── timedate
│   │   ├── hwclock-util.c
│   │   ├── hwclock-util.h
│   │   ├── meson.build
│   │   ├── org.freedesktop.timedate1.conf
│   │   ├── org.freedesktop.timedate1.policy
│   │   ├── org.freedesktop.timedate1.service
│   │   ├── timedatectl.c
│   │   └── timedated.c
│   ├── timesync
│   │   ├── 80-systemd-timesync.list
│   │   ├── meson.build
│   │   ├── org.freedesktop.timesync1.conf
│   │   ├── org.freedesktop.timesync1.policy
│   │   ├── org.freedesktop.timesync1.service
│   │   ├── test-timesync.c
│   │   ├── timesyncd-bus.c
│   │   ├── timesyncd-bus.h
│   │   ├── timesyncd-conf.c
│   │   ├── timesyncd-conf.h
│   │   ├── timesyncd-forward.h
│   │   ├── timesyncd-gperf.gperf
│   │   ├── timesyncd-manager.c
│   │   ├── timesyncd-manager.h
│   │   ├── timesyncd-ntp-message.h
│   │   ├── timesyncd-server.c
│   │   ├── timesyncd-server.h
│   │   ├── timesyncd.c
│   │   ├── timesyncd.conf.in
│   │   └── wait-sync.c
│   ├── tmpfiles
│   │   ├── meson.build
│   │   ├── offline-passwd.c
│   │   ├── offline-passwd.h
│   │   ├── test-offline-passwd.c
│   │   └── tmpfiles.c
│   ├── tpm2-setup
│   │   ├── meson.build
│   │   ├── tpm2-clear.c
│   │   ├── tpm2-generator.c
│   │   └── tpm2-setup.c
│   ├── tty-ask-password-agent
│   │   ├── meson.build
│   │   └── tty-ask-password-agent.c
│   ├── udev
│   │   ├── ata_id
│   │   │   └── ata_id.c
│   │   ├── cdrom_id
│   │   │   └── cdrom_id.c
│   │   ├── dmi_memory_id
│   │   │   └── dmi_memory_id.c
│   │   ├── fido_id
│   │   │   ├── fido_id_desc.c
│   │   │   ├── fido_id_desc.h
│   │   │   ├── fido_id.c
│   │   │   ├── fuzz-fido-id-desc.c
│   │   │   └── test-fido-id-desc.c
│   │   ├── fuzz-udev-rule-parse-value.c
│   │   ├── fuzz-udev-rules.c
│   │   ├── fuzz-udev-rules.options
│   │   ├── generate-keyboard-keys-gperf.sh
│   │   ├── generate-keyboard-keys-list.sh
│   │   ├── iocost
│   │   │   ├── iocost.c
│   │   │   └── iocost.conf
│   │   ├── meson.build
│   │   ├── mtd_probe
│   │   │   ├── mtd_probe.c
│   │   │   ├── mtd_probe.h
│   │   │   └── probe_smartmedia.c
│   │   ├── net
│   │   │   ├── fuzz-link-parser.c
│   │   │   ├── fuzz-link-parser.options
│   │   │   ├── link-config-gperf.gperf
│   │   │   ├── link-config.c
│   │   │   ├── link-config.h
│   │   │   └── test-link-config-tables.c
│   │   ├── NOTES.md
│   │   ├── scsi_id
│   │   │   ├── README
│   │   │   ├── scsi_id.c
│   │   │   ├── scsi_id.h
│   │   │   ├── scsi_serial.c
│   │   │   └── scsi.h
│   │   ├── test-udev-builtin.c
│   │   ├── test-udev-format.c
│   │   ├── test-udev-manager.c
│   │   ├── test-udev-node.c
│   │   ├── test-udev-rule-runner.c
│   │   ├── test-udev-rules.c
│   │   ├── test-udev-spawn.c
│   │   ├── udev-builtin-blkid.c
│   │   ├── udev-builtin-btrfs.c
│   │   ├── udev-builtin-dissect_image.c
│   │   ├── udev-builtin-factory_reset.c
│   │   ├── udev-builtin-hwdb.c
│   │   ├── udev-builtin-input_id.c
│   │   ├── udev-builtin-keyboard.c
│   │   ├── udev-builtin-kmod.c
│   │   ├── udev-builtin-net_driver.c
│   │   ├── udev-builtin-net_id.c
│   │   ├── udev-builtin-net_setup_link.c
│   │   ├── udev-builtin-path_id.c
│   │   ├── udev-builtin-uaccess.c
│   │   ├── udev-builtin-usb_id.c
│   │   ├── udev-builtin.c
│   │   ├── udev-builtin.h
│   │   ├── udev-config.c
│   │   ├── udev-config.h
│   │   ├── udev-ctrl.c
│   │   ├── udev-ctrl.h
│   │   ├── udev-def.h
│   │   ├── udev-dump.c
│   │   ├── udev-dump.h
│   │   ├── udev-error.c
│   │   ├── udev-error.h
│   │   ├── udev-event.c
│   │   ├── udev-event.h
│   │   ├── udev-format.c
│   │   ├── udev-format.h
│   │   ├── udev-forward.h
│   │   ├── udev-manager-ctrl.c
│   │   ├── udev-manager-ctrl.h
│   │   ├── udev-manager.c
│   │   ├── udev-manager.h
│   │   ├── udev-node.c
│   │   ├── udev-node.h
│   │   ├── udev-rules.c
│   │   ├── udev-rules.h
│   │   ├── udev-spawn.c
│   │   ├── udev-spawn.h
│   │   ├── udev-trace.h
│   │   ├── udev-varlink.c
│   │   ├── udev-varlink.h
│   │   ├── udev-watch.c
│   │   ├── udev-watch.h
│   │   ├── udev-worker.c
│   │   ├── udev-worker.h
│   │   ├── udev.conf
│   │   ├── udev.pc.in
│   │   ├── udevadm-cat.c
│   │   ├── udevadm-control.c
│   │   ├── udevadm-hwdb.c
│   │   ├── udevadm-info.c
│   │   ├── udevadm-lock.c
│   │   ├── udevadm-monitor.c
│   │   ├── udevadm-settle.c
│   │   ├── udevadm-test-builtin.c
│   │   ├── udevadm-test.c
│   │   ├── udevadm-trigger.c
│   │   ├── udevadm-util.c
│   │   ├── udevadm-util.h
│   │   ├── udevadm-verify.c
│   │   ├── udevadm-wait.c
│   │   ├── udevadm.c
│   │   ├── udevadm.h
│   │   ├── udevd.c
│   │   ├── udevd.h
│   │   └── v4l_id
│   │       └── v4l_id.c
│   ├── ukify
│   │   ├── test
│   │   │   ├── example.signing.crt.base64
│   │   │   ├── example.signing.key.base64
│   │   │   ├── example.tpm2-pcr-private.pem.base64
│   │   │   ├── example.tpm2-pcr-private2.pem.base64
│   │   │   ├── example.tpm2-pcr-public.pem.base64
│   │   │   ├── example.tpm2-pcr-public2.pem.base64
│   │   │   ├── meson.build
│   │   │   ├── pytest.ini
│   │   │   └── test_ukify.py
│   │   └── ukify.py
│   ├── update-done
│   │   ├── meson.build
│   │   └── update-done.c
│   ├── update-utmp
│   │   ├── meson.build
│   │   └── update-utmp.c
│   ├── user-sessions
│   │   ├── meson.build
│   │   └── user-sessions.c
│   ├── userdb
│   │   ├── 20-systemd-userdb.conf.in
│   │   ├── meson.build
│   │   ├── userdbctl.c
│   │   ├── userdbd-manager.c
│   │   ├── userdbd-manager.h
│   │   ├── userdbd.c
│   │   └── userwork.c
│   ├── validatefs
│   │   ├── meson.build
│   │   └── validatefs.c
│   ├── varlinkctl
│   │   ├── meson.build
│   │   └── varlinkctl.c
│   ├── vconsole
│   │   ├── meson.build
│   │   └── vconsole-setup.c
│   ├── veritysetup
│   │   ├── meson.build
│   │   ├── veritysetup-generator.c
│   │   └── veritysetup.c
│   ├── version
│   │   ├── meson.build
│   │   └── version.h.in
│   ├── vmspawn
│   │   ├── meson.build
│   │   ├── test-vmspawn-util.c
│   │   ├── vmspawn-mount.c
│   │   ├── vmspawn-mount.h
│   │   ├── vmspawn-register.c
│   │   ├── vmspawn-register.h
│   │   ├── vmspawn-scope.c
│   │   ├── vmspawn-scope.h
│   │   ├── vmspawn-settings.c
│   │   ├── vmspawn-settings.h
│   │   ├── vmspawn-util.c
│   │   ├── vmspawn-util.h
│   │   └── vmspawn.c
│   ├── volatile-root
│   │   ├── meson.build
│   │   └── volatile-root.c
│   ├── vpick
│   │   ├── meson.build
│   │   └── vpick-tool.c
│   └── xdg-autostart-generator
│       ├── fuzz-xdg-desktop.c
│       ├── fuzz-xdg-desktop.options
│       ├── meson.build
│       ├── test-xdg-autostart.c
│       ├── xdg-autostart-condition.c
│       ├── xdg-autostart-generator.c
│       ├── xdg-autostart-service.c
│       └── xdg-autostart-service.h
├── sysctl.d
│   ├── 50-coredump.conf.in
│   ├── 50-default.conf
│   ├── 50-pid-max.conf
│   ├── meson.build
│   └── README
├── sysusers.d
│   ├── basic.conf.in
│   ├── meson.build
│   ├── README
│   ├── systemd-coredump.conf
│   ├── systemd-journal.conf.in
│   ├── systemd-network.conf.in
│   ├── systemd-oom.conf
│   ├── systemd-remote.conf
│   ├── systemd-resolve.conf.in
│   └── systemd-timesync.conf.in
├── test
│   ├── auxv
│   │   ├── bash.riscv64
│   │   ├── cat.s390x
│   │   ├── dbus-broker-launch.aarch64
│   │   ├── dbus-broker-launch.amd64
│   │   ├── polkitd.aarch64
│   │   ├── resolved.arm32
│   │   ├── sleep.i686
│   │   ├── sleep32.i686
│   │   ├── sleep64.amd64
│   │   ├── sudo.aarch64
│   │   └── sudo.amd64
│   ├── create-sys-script.py
│   ├── dmidecode-dumps
│   │   ├── HP-Z600.bin
│   │   ├── HP-Z600.bin.txt
│   │   ├── Lenovo-Thinkcentre-m720s.bin
│   │   ├── Lenovo-Thinkcentre-m720s.bin.txt
│   │   ├── Lenovo-ThinkPad-X280.bin
│   │   └── Lenovo-ThinkPad-X280.bin.txt
│   ├── fuzz
│   │   ├── fuzz-bootspec
│   │   │   ├── crash-autoentry
│   │   │   ├── crash-empty-value
│   │   │   ├── crash-json-dispatch
│   │   │   ├── oss-fuzz-53578
│   │   │   ├── sample1
│   │   │   └── sanitizer-overload
│   │   ├── fuzz-bus-match
│   │   │   ├── bugzilla1935084.input
│   │   │   └── test.input
│   │   ├── fuzz-bus-message
│   │   │   ├── crash-array
│   │   │   ├── crash-array-field-skip
│   │   │   ├── crash-array-offset
│   │   │   ├── crash-empty-string
│   │   │   ├── crash-empty-struct
│   │   │   ├── crash-mem-overread
│   │   │   ├── crash-nesting
│   │   │   ├── crash-offset-table
│   │   │   ├── crash-return-value
│   │   │   ├── crash-return-value-again
│   │   │   ├── crash-unsigned-wraparound
│   │   │   ├── issue-23486-case-1
│   │   │   ├── issue-23486-case-2
│   │   │   ├── issue-23486-case-3
│   │   │   ├── leak-container-exit
│   │   │   ├── message1
│   │   │   ├── oss-fuzz-14016
│   │   │   ├── oss-fuzz-19446
│   │   │   ├── timeout-empty-struct
│   │   │   └── zero-offset-to-null-pointer
│   │   ├── fuzz-calendarspec
│   │   │   ├── cant-parse-printed
│   │   │   ├── corpus
│   │   │   ├── crash-parse-star-non-star
│   │   │   ├── input1
│   │   │   ├── oss-fuzz-14108
│   │   │   ├── oss-fuzz-22208
│   │   │   └── print-loses-spec
│   │   ├── fuzz-catalog
│   │   │   ├── language-too-short
│   │   │   └── systemd.pl.catalog
│   │   ├── fuzz-compress
│   │   │   └── issue-36472
│   │   ├── fuzz-dhcp-client
│   │   │   ├── dnr_invalid
│   │   │   ├── dnr_v4
│   │   │   ├── parse-memleak
│   │   │   └── timeout-lease_parse_routes
│   │   ├── fuzz-dhcp-server
│   │   │   ├── buffer-overflow-1
│   │   │   ├── buffer-overflow-2
│   │   │   ├── discover-existing
│   │   │   ├── discover-new
│   │   │   ├── duplicate-input-data
│   │   │   ├── release
│   │   │   ├── request-existing
│   │   │   ├── request-new
│   │   │   ├── request-reboot
│   │   │   └── request-renew
│   │   ├── fuzz-dhcp-server-relay
│   │   │   ├── sample1
│   │   │   ├── sample2
│   │   │   └── too-large-packet
│   │   ├── fuzz-dhcp6-client
│   │   │   ├── crash-13578
│   │   │   ├── crash-13591
│   │   │   ├── crash-buf-size
│   │   │   ├── crash-domainname
│   │   │   ├── crash-initial1
│   │   │   ├── crash-initial2
│   │   │   ├── crash-initial3
│   │   │   ├── dnr_v6
│   │   │   ├── oss-fuzz-10746
│   │   │   └── oss-fuzz-11019
│   │   ├── fuzz-dns-packet
│   │   │   ├── crash-null
│   │   │   ├── issue-7888
│   │   │   ├── oss-fuzz-13422
│   │   │   ├── oss-fuzz-19227
│   │   │   └── oss-fuzz-5465
│   │   ├── fuzz-env-file
│   │   │   └── simple-env-file
│   │   ├── fuzz-etc-hosts
│   │   │   ├── oss-fuzz-47708
│   │   │   └── timeout-strv
│   │   ├── fuzz-execute-serialize
│   │   │   ├── crash-395e
│   │   │   ├── crash-622a
│   │   │   ├── initial
│   │   │   ├── mount-images
│   │   │   ├── oss-fuzz-429112745
│   │   │   └── state
│   │   ├── fuzz-fido-id-desc
│   │   │   ├── crash0
│   │   │   ├── crash1
│   │   │   ├── report0
│   │   │   └── report1
│   │   ├── fuzz-journal-remote
│   │   │   ├── crash-nul-in-field-name
│   │   │   ├── crash-source-realtime-ts
│   │   │   ├── invalid-ts.txt
│   │   │   ├── oss-fuzz-21122
│   │   │   ├── oss-fuzz-25353
│   │   │   ├── oss-fuzz-28817
│   │   │   ├── oss-fuzz-385221809
│   │   │   ├── oss-fuzz-8658
│   │   │   ├── oss-fuzz-8659
│   │   │   ├── oss-fuzz-8686
│   │   │   ├── oss-fuzz-9341
│   │   │   └── sample.txt
│   │   ├── fuzz-journald-audit
│   │   │   ├── basic
│   │   │   └── crash
│   │   ├── fuzz-journald-kmsg
│   │   │   ├── basic
│   │   │   ├── crash-ident-with-spaces
│   │   │   ├── dev-null
│   │   │   ├── leak-missing-cleanup
│   │   │   ├── loopback
│   │   │   ├── oss-fuzz-33881
│   │   │   └── subsystem-loopback
│   │   ├── fuzz-journald-native-fd
│   │   │   └── basic
│   │   ├── fuzz-journald-stream
│   │   │   └── basic
│   │   ├── fuzz-journald-syslog
│   │   │   ├── github-9795
│   │   │   ├── github-9820
│   │   │   ├── github-9827
│   │   │   └── github-9829
│   │   ├── fuzz-json
│   │   │   ├── crash-5639441482252288
│   │   │   ├── github-15907
│   │   │   ├── leak-normalize-fail
│   │   │   ├── leak-normalize-object
│   │   │   ├── leak-sort
│   │   │   └── oss-fuzz-10908
│   │   ├── fuzz-link-parser
│   │   │   ├── 99-default.link
│   │   │   ├── advertise-segv.link
│   │   │   ├── condition-memleak.link
│   │   │   ├── oss-fuzz-13878
│   │   │   └── oss-fuzz-13882
│   │   ├── fuzz-lldp-rx
│   │   │   ├── basic
│   │   │   ├── incomplete
│   │   │   └── oui
│   │   ├── fuzz-manager-serialize
│   │   │   ├── activation-details
│   │   │   ├── bogus-unit-type
│   │   │   ├── empty-attachment-path
│   │   │   ├── invalid-varlink-sock
│   │   │   ├── netns-invalid-socket
│   │   │   ├── service-accept-socket
│   │   │   ├── socket-int-max
│   │   │   └── state
│   │   ├── fuzz-ndisc-rs
│   │   │   ├── encrypted-dns
│   │   │   ├── infinite-loop-recv
│   │   │   └── infinite-loop-timeout
│   │   ├── fuzz-netdev-parser
│   │   │   ├── 6rd-tunnel.netdev
│   │   │   ├── batadv.netdev
│   │   │   ├── bond-backup.netdev
│   │   │   ├── bond.netdev
│   │   │   ├── bridge-2.netdev
│   │   │   ├── bridge.netdev
│   │   │   ├── crash-null-address
│   │   │   ├── dummy-2.netdev
│   │   │   ├── dummy.netdev
│   │   │   ├── erspan-tunnel.netdev
│   │   │   ├── geneve.netdev
│   │   │   ├── github-10615
│   │   │   ├── github-10629
│   │   │   ├── github-15968
│   │   │   ├── gre-tunnel.netdev
│   │   │   ├── gretap-tunnel.netdev
│   │   │   ├── ip6gre-tunnel.netdev
│   │   │   ├── ip6tnl-tunnel.netdev
│   │   │   ├── ipip-tunnel.netdev
│   │   │   ├── ipip-tunnel2.netdev
│   │   │   ├── ipvlan.netdev
│   │   │   ├── macvlan.netdev
│   │   │   ├── macvtap.netdev
│   │   │   ├── oss-fuzz-11279
│   │   │   ├── oss-fuzz-11280
│   │   │   ├── oss-fuzz-11286
│   │   │   ├── oss-fuzz-11287
│   │   │   ├── oss-fuzz-11296
│   │   │   ├── oss-fuzz-11297
│   │   │   ├── oss-fuzz-11299
│   │   │   ├── oss-fuzz-11324
│   │   │   ├── oss-fuzz-11344
│   │   │   ├── oss-fuzz-13719
│   │   │   ├── oss-fuzz-13884
│   │   │   ├── oss-fuzz-13886
│   │   │   ├── oss-fuzz-14157
│   │   │   ├── oss-fuzz-14158
│   │   │   ├── oss-fuzz-22547
│   │   │   ├── oss-fuzz-62556
│   │   │   ├── sit-tunnel.netdev
│   │   │   ├── tap.netdev
│   │   │   ├── tun.netdev
│   │   │   ├── vcan.netdev
│   │   │   ├── veth.netdev
│   │   │   ├── vlan.netdev
│   │   │   ├── vrf.netdev
│   │   │   ├── vti-tunnel.netdev
│   │   │   ├── vti6-tunnel.netdev
│   │   │   ├── vxlan.netdev
│   │   │   ├── wg-dup-endpoint
│   │   │   ├── wireguard.netdev
│   │   │   └── xfrm.netdev
│   │   ├── fuzz-network-parser
│   │   │   ├── active-slave
│   │   │   ├── address-link-section
│   │   │   ├── address-section
│   │   │   ├── address-section-misc
│   │   │   ├── bond199
│   │   │   ├── bridge-slave-interface-1
│   │   │   ├── bridge-slave-interface-2
│   │   │   ├── bridge99
│   │   │   ├── configure-no-carrier
│   │   │   ├── dhcp-client
│   │   │   ├── dhcp-client-anonymize
│   │   │   ├── dhcp-client-ipv4-no-ipv6
│   │   │   ├── dhcp-client-ipv4-only
│   │   │   ├── dhcp-client-ipv6-only
│   │   │   ├── dhcp-client-listen-port
│   │   │   ├── dhcp-client-route-metric
│   │   │   ├── dhcp-client-route-table
│   │   │   ├── dhcp-client-tz-router
│   │   │   ├── dhcp-critical-connection
│   │   │   ├── dhcp-option
│   │   │   ├── dhcp-server
│   │   │   ├── dhcp-server-static-lease
│   │   │   ├── dhcp-server-tz-router
│   │   │   ├── dhcp-server-veth-peer
│   │   │   ├── dhcp-v4-server-veth-peer
│   │   │   ├── dhcpv4-client-settings
│   │   │   ├── dhcpv6-rapid-commit
│   │   │   ├── dns-trust-dup-anchor
│   │   │   ├── emit-lldp
│   │   │   ├── fibrule-port-range
│   │   │   ├── github-10639
│   │   │   ├── github-13938
│   │   │   ├── github-15885
│   │   │   ├── github-15951
│   │   │   ├── gretap
│   │   │   ├── gretun
│   │   │   ├── ip6gretap
│   │   │   ├── ip6tnl
│   │   │   ├── ipip
│   │   │   ├── ipv6-address-label
│   │   │   ├── ipv6-prefix
│   │   │   ├── ipv6-prefix-veth
│   │   │   ├── ipvlan
│   │   │   ├── link-section-unmanaged
│   │   │   ├── lldp
│   │   │   ├── macvlan
│   │   │   ├── macvtap
│   │   │   ├── neighbor-section
│   │   │   ├── oss-fuzz-11285
│   │   │   ├── oss-fuzz-11302
│   │   │   ├── oss-fuzz-11314
│   │   │   ├── oss-fuzz-11345
│   │   │   ├── oss-fuzz-13059
│   │   │   ├── oss-fuzz-13354
│   │   │   ├── oss-fuzz-13433
│   │   │   ├── oss-fuzz-13888
│   │   │   ├── oss-fuzz-15678
│   │   │   ├── oss-fuzz-20548
│   │   │   ├── oss-fuzz-23895
│   │   │   ├── oss-fuzz-23950
│   │   │   ├── oss-fuzz-372994449
│   │   │   ├── oss-fuzz-391916479
│   │   │   ├── primary-slave
│   │   │   ├── route-section
│   │   │   ├── route-type
│   │   │   ├── routing-policy-rule
│   │   │   ├── search-domain
│   │   │   ├── sit
│   │   │   ├── sysctl
│   │   │   ├── tcp-window-settings
│   │   │   ├── test-static
│   │   │   ├── test1-bond199
│   │   │   ├── vlan
│   │   │   ├── vti
│   │   │   ├── vti6
│   │   │   ├── vxlan
│   │   │   └── xfrm
│   │   ├── fuzz-nspawn-oci
│   │   │   ├── basic.json
│   │   │   ├── double-free
│   │   │   ├── invalid-read-magic-string
│   │   │   ├── invalid-read-magic-string2
│   │   │   └── no-mount-source
│   │   ├── fuzz-nspawn-settings
│   │   │   ├── basic-config
│   │   │   ├── leak-bind-mount
│   │   │   └── oss-fuzz-13691
│   │   ├── fuzz-resource-record
│   │   │   ├── just-slash
│   │   │   ├── oss-fuzz-54059
│   │   │   ├── oss-fuzz-54065
│   │   │   ├── oss-fuzz-54080
│   │   │   ├── oss-fuzz-54090
│   │   │   └── ub-zero-length-rdata
│   │   ├── fuzz-systemctl-parse-argv
│   │   │   ├── help.input
│   │   │   ├── missing-strv-free
│   │   │   ├── oss-fuzz-31055
│   │   │   ├── oss-fuzz-31714
│   │   │   ├── oss-fuzz-56915
│   │   │   └── oss-fuzz-70153
│   │   ├── fuzz-udev-database
│   │   │   └── sample.txt
│   │   ├── fuzz-udev-rules
│   │   │   ├── block.rules
│   │   │   ├── btrfs.rules
│   │   │   ├── cdrom_id.rules
│   │   │   ├── drivers.rules
│   │   │   ├── drm.rules
│   │   │   ├── evdev.rules
│   │   │   ├── input-id.rules
│   │   │   ├── joystick.rules
│   │   │   ├── line-too-long
│   │   │   ├── mouse.rules
│   │   │   ├── net-description.rules
│   │   │   ├── net-setup-link.rules
│   │   │   ├── oss-fuzz-12980
│   │   │   ├── persistent-alsa.rules
│   │   │   ├── persistent-input.rules
│   │   │   ├── persistent-storage.rules
│   │   │   ├── persistent-v4l.rules
│   │   │   ├── probe_mtd.rules
│   │   │   ├── sensor.rules
│   │   │   ├── serial.rules
│   │   │   ├── sound-card.rules
│   │   │   ├── storage-tape.rules
│   │   │   ├── systemd.rules
│   │   │   ├── touchpad.rules
│   │   │   └── udev-default.rules
│   │   ├── fuzz-unit-file
│   │   │   ├── ask-password-console.path
│   │   │   ├── binfmt_misc.automount
│   │   │   ├── directives-all.service
│   │   │   ├── dm-back\x2dslash.swap
│   │   │   ├── empty.scope
│   │   │   ├── github-19178
│   │   │   ├── machine.slice
│   │   │   ├── oss-fuzz-10007
│   │   │   ├── oss-fuzz-11569
│   │   │   ├── oss-fuzz-13125
│   │   │   ├── oss-fuzz-32991
│   │   │   ├── oss-fuzz-33270
│   │   │   ├── oss-fuzz-33876
│   │   │   ├── oss-fuzz-6884
│   │   │   ├── oss-fuzz-6885
│   │   │   ├── oss-fuzz-6886
│   │   │   ├── oss-fuzz-6892
│   │   │   ├── oss-fuzz-6897
│   │   │   ├── oss-fuzz-6897-evverx
│   │   │   ├── oss-fuzz-6908
│   │   │   ├── oss-fuzz-6917
│   │   │   ├── oss-fuzz-6977
│   │   │   ├── oss-fuzz-6977-unminimized
│   │   │   ├── oss-fuzz-7004
│   │   │   ├── oss-fuzz-8064
│   │   │   ├── oss-fuzz-8827
│   │   │   ├── syslog.socket
│   │   │   ├── systemd-machined.service
│   │   │   ├── systemd-resolved.service
│   │   │   ├── timers.target
│   │   │   ├── tmpfiles-clean.timer
│   │   │   └── var-lib-machines.mount
│   │   ├── fuzz-varlink
│   │   │   ├── array
│   │   │   ├── do-something
│   │   │   ├── huge-method
│   │   │   ├── method-call
│   │   │   ├── method-error
│   │   │   ├── method-reply
│   │   │   ├── oss-fuzz-14688
│   │   │   ├── oss-fuzz-14708
│   │   │   └── timeout
│   │   ├── fuzz-varlink-idl
│   │   │   ├── crash-d1860f2b
│   │   │   ├── interface1
│   │   │   └── oss-fuzz-69730
│   │   ├── fuzz-xdg-desktop
│   │   │   ├── full.desktop
│   │   │   ├── oss-fuzz-22812
│   │   │   ├── SettingsDaemon.desktop
│   │   │   └── valid.desktop
│   │   ├── generate-directives.py
│   │   └── meson.build
│   ├── hwdb-test.sh
│   ├── hwdb.d
│   │   └── 10-bad.hwdb
│   ├── integration-test-setup.sh
│   ├── integration-tests
│   │   ├── integration-test-wrapper.py
│   │   ├── meson.build
│   │   ├── README.md
│   │   ├── standalone
│   │   │   ├── integration-tests -> ..
│   │   │   └── meson.build
│   │   ├── TEST-01-BASIC
│   │   │   └── meson.build
│   │   ├── TEST-02-UNITTESTS
│   │   │   └── meson.build
│   │   ├── TEST-03-JOBS
│   │   │   ├── meson.build
│   │   │   └── TEST-03-JOBS.units
│   │   │       ├── always-activating.service
│   │   │       ├── always-activating.socket
│   │   │       ├── counter.service
│   │   │       ├── counter.sh
│   │   │       ├── fails-on-restart-restartdirect.service
│   │   │       ├── fails-on-restart-restartdirect.target
│   │   │       ├── fails-on-restart.service
│   │   │       ├── fails-on-restart.target
│   │   │       ├── hello-after-sleep.target
│   │   │       ├── hello.service
│   │   │       ├── propagatestopto-and-pullin.target
│   │   │       ├── propagatestopto-indirect.target
│   │   │       ├── propagatestopto-only.target
│   │   │       ├── restart-on-failure.service
│   │   │       ├── sleep-infinity-restart-direct.service
│   │   │       ├── sleep-infinity-restart-normal.service
│   │   │       ├── sleep-infinity-simple.service
│   │   │       ├── sleep.service
│   │   │       ├── succeeds-on-restart-restartdirect.service
│   │   │       ├── succeeds-on-restart-restartdirect.target
│   │   │       ├── succeeds-on-restart.service
│   │   │       ├── succeeds-on-restart.sh
│   │   │       ├── succeeds-on-restart.target
│   │   │       └── unstoppable.service
│   │   ├── TEST-04-JOURNAL
│   │   │   ├── meson.build
│   │   │   └── TEST-04-JOURNAL.units
│   │   │       ├── delegated-cgroup-filtering.service
│   │   │       ├── forever-print-hola.service
│   │   │       ├── logs-filtering.service
│   │   │       ├── silent-success.service
│   │   │       └── verbose-success.service
│   │   ├── TEST-05-RLIMITS
│   │   │   └── meson.build
│   │   ├── TEST-06-SELINUX
│   │   │   ├── meson.build
│   │   │   └── TEST-06-SELINUX.units
│   │   │       └── hola.service
│   │   ├── TEST-07-PID1
│   │   │   ├── meson.build
│   │   │   └── TEST-07-PID1.units
│   │   │       ├── issue14566-repro.service
│   │   │       ├── issue14566-repro.sh
│   │   │       ├── issue16115-repro-1.service
│   │   │       ├── issue16115-repro-2.service
│   │   │       ├── issue16115-repro-3.service
│   │   │       ├── issue2467.service
│   │   │       ├── issue2467.socket
│   │   │       ├── issue2730-alias.mount -> issue2730.mount
│   │   │       ├── issue2730.mount
│   │   │       ├── issue27953.service
│   │   │       ├── issue3166-fail-on-restart.service
│   │   │       ├── local-fs.target.wants
│   │   │       │   └── issue2730.mount -> ../issue2730.mount
│   │   │       ├── pass-fds-to-exec-no.socket
│   │   │       ├── pass-fds-to-exec-yes.socket
│   │   │       └── prefix-shell.service
│   │   ├── TEST-08-INITRD
│   │   │   └── meson.build
│   │   ├── TEST-09-REBOOT
│   │   │   └── meson.build
│   │   ├── TEST-13-NSPAWN
│   │   │   └── meson.build
│   │   ├── TEST-15-DROPIN
│   │   │   └── meson.build
│   │   ├── TEST-16-EXTEND-TIMEOUT
│   │   │   ├── meson.build
│   │   │   └── TEST-16-EXTEND-TIMEOUT.units
│   │   │       ├── extend-timeout.sh
│   │   │       ├── fail-runtime.service
│   │   │       ├── fail-start.service
│   │   │       ├── fail-stop.service
│   │   │       ├── success-all.service
│   │   │       ├── success-runtime.service
│   │   │       ├── success-start.service
│   │   │       └── success-stop.service
│   │   ├── TEST-17-UDEV
│   │   │   ├── deny-list-ubuntu-ci-ppc64el
│   │   │   └── meson.build
│   │   ├── TEST-18-FAILUREACTION
│   │   │   └── meson.build
│   │   ├── TEST-19-CGROUP
│   │   │   └── meson.build
│   │   ├── TEST-21-DFUZZER
│   │   │   └── meson.build
│   │   ├── TEST-22-TMPFILES
│   │   │   └── meson.build
│   │   ├── TEST-23-UNIT-FILE
│   │   │   ├── meson.build
│   │   │   └── TEST-23-UNIT-FILE.units
│   │   │       ├── TEST-23-UNIT-FILE-binds-to.service
│   │   │       ├── TEST-23-UNIT-FILE-bound-by.service
│   │   │       ├── TEST-23-UNIT-FILE-fail.service
│   │   │       ├── TEST-23-UNIT-FILE-joins-namespace-of-1.service
│   │   │       ├── TEST-23-UNIT-FILE-joins-namespace-of-2.service
│   │   │       ├── TEST-23-UNIT-FILE-joins-namespace-of-3.service
│   │   │       ├── TEST-23-UNIT-FILE-joins-namespace-of-4.service
│   │   │       ├── TEST-23-UNIT-FILE-joins-namespace-of-5.service
│   │   │       ├── TEST-23-UNIT-FILE-joins-namespace-of-6.service
│   │   │       ├── TEST-23-UNIT-FILE-joins-namespace-of-7.service
│   │   │       ├── TEST-23-UNIT-FILE-joins-namespace-of-8.service
│   │   │       ├── TEST-23-UNIT-FILE-joins-namespace-of-9.service
│   │   │       ├── TEST-23-UNIT-FILE-namespaced.service
│   │   │       ├── TEST-23-UNIT-FILE-non-namespaced.service
│   │   │       ├── TEST-23-UNIT-FILE-oneshot-restartforce.sh
│   │   │       ├── TEST-23-UNIT-FILE-openfile-server.socket
│   │   │       ├── TEST-23-UNIT-FILE-openfile-server@.service
│   │   │       ├── TEST-23-UNIT-FILE-prop-stop-one.service
│   │   │       ├── TEST-23-UNIT-FILE-prop-stop-two.service
│   │   │       ├── TEST-23-UNIT-FILE-retry-fail.service
│   │   │       ├── TEST-23-UNIT-FILE-retry-upheld.service
│   │   │       ├── TEST-23-UNIT-FILE-retry-uphold.service
│   │   │       ├── TEST-23-UNIT-FILE-short-lived.service
│   │   │       ├── TEST-23-UNIT-FILE-specifier-j-depends-wants.service
│   │   │       ├── TEST-23-UNIT-FILE-specifier-j-wants.service
│   │   │       ├── TEST-23-UNIT-FILE-success.service
│   │   │       ├── TEST-23-UNIT-FILE-upheldby-install.service
│   │   │       └── TEST-23-UNIT-FILE-uphold.service
│   │   ├── TEST-24-CRYPTSETUP
│   │   │   └── meson.build
│   │   ├── TEST-25-IMPORT
│   │   │   └── meson.build
│   │   ├── TEST-26-SYSTEMCTL
│   │   │   └── meson.build
│   │   ├── TEST-29-PORTABLE
│   │   │   └── meson.build
│   │   ├── TEST-30-ONCLOCKCHANGE
│   │   │   ├── meson.build
│   │   │   └── TEST-30-ONCLOCKCHANGE.units
│   │   │       └── systemd-timedated.service.d
│   │   │           └── watchdog.conf
│   │   ├── TEST-31-DEVICE-ENUMERATION
│   │   │   └── meson.build
│   │   ├── TEST-32-OOMPOLICY
│   │   │   └── meson.build
│   │   ├── TEST-34-DYNAMICUSERMIGRATE
│   │   │   └── meson.build
│   │   ├── TEST-35-LOGIN
│   │   │   └── meson.build
│   │   ├── TEST-36-NUMAPOLICY
│   │   │   └── meson.build
│   │   ├── TEST-38-FREEZER
│   │   │   └── meson.build
│   │   ├── TEST-43-PRIVATEUSER-UNPRIV
│   │   │   └── meson.build
│   │   ├── TEST-44-LOG-NAMESPACE
│   │   │   └── meson.build
│   │   ├── TEST-45-TIMEDATE
│   │   │   └── meson.build
│   │   ├── TEST-46-HOMED
│   │   │   └── meson.build
│   │   ├── TEST-50-DISSECT
│   │   │   └── meson.build
│   │   ├── TEST-52-HONORFIRSTSHUTDOWN
│   │   │   ├── meson.build
│   │   │   └── TEST-52-HONORFIRSTSHUTDOWN.units
│   │   │       ├── test-honor-first-shutdown.service
│   │   │       └── test-honor-first-shutdown.sh
│   │   ├── TEST-53-ISSUE-16347
│   │   │   └── meson.build
│   │   ├── TEST-54-CREDS
│   │   │   ├── meson.build
│   │   │   ├── systemd.extra-unit.my-service.service
│   │   │   ├── systemd.unit-dropin.my-service.service
│   │   │   └── systemd.unit-dropin.my-service.service~30-named.service
│   │   ├── TEST-55-OOMD
│   │   │   ├── meson.build
│   │   │   └── systemd.unit-dropin.init.scope
│   │   ├── TEST-58-REPART
│   │   │   └── meson.build
│   │   ├── TEST-59-RELOADING-RESTART
│   │   │   └── meson.build
│   │   ├── TEST-60-MOUNT-RATELIMIT
│   │   │   └── meson.build
│   │   ├── TEST-62-RESTRICT-IFACES
│   │   │   └── meson.build
│   │   ├── TEST-63-PATH
│   │   │   ├── meson.build
│   │   │   └── TEST-63-PATH.units
│   │   │       ├── test63-glob.path
│   │   │       ├── test63-glob.service
│   │   │       ├── test63-issue-24577-dep.service
│   │   │       ├── test63-issue-24577.path
│   │   │       ├── test63-issue-24577.service
│   │   │       ├── test63-pr-30768.path
│   │   │       ├── test63-pr-30768.service
│   │   │       ├── test63.path
│   │   │       └── test63.service
│   │   ├── TEST-64-UDEV-STORAGE
│   │   │   ├── deny-list-ubuntu-ci
│   │   │   └── meson.build
│   │   ├── TEST-65-ANALYZE
│   │   │   └── meson.build
│   │   ├── TEST-66-DEVICE-ISOLATION
│   │   │   └── meson.build
│   │   ├── TEST-67-INTEGRITY
│   │   │   └── meson.build
│   │   ├── TEST-68-PROPAGATE-EXIT-STATUS
│   │   │   └── meson.build
│   │   ├── TEST-69-SHUTDOWN
│   │   │   └── meson.build
│   │   ├── TEST-70-TPM2
│   │   │   └── meson.build
│   │   ├── TEST-71-HOSTNAME
│   │   │   └── meson.build
│   │   ├── TEST-72-SYSUPDATE
│   │   │   └── meson.build
│   │   ├── TEST-73-LOCALE
│   │   │   └── meson.build
│   │   ├── TEST-74-AUX-UTILS
│   │   │   ├── meson.build
│   │   │   └── TEST-74-AUX-UTILS.units
│   │   │       ├── realtime-test.service
│   │   │       └── realtime-test.timer
│   │   ├── TEST-75-RESOLVED
│   │   │   └── meson.build
│   │   ├── TEST-76-SYSCTL
│   │   │   └── meson.build
│   │   ├── TEST-78-SIGQUEUE
│   │   │   └── meson.build
│   │   ├── TEST-79-MEMPRESS
│   │   │   └── meson.build
│   │   ├── TEST-80-NOTIFYACCESS
│   │   │   ├── meson.build
│   │   │   └── TEST-80-NOTIFYACCESS.units
│   │   │       ├── fdstore-nopin.service
│   │   │       ├── fdstore-pin.service
│   │   │       ├── fdstore-pin.sh
│   │   │       ├── fdstore-pin.target
│   │   │       ├── notify.service
│   │   │       └── test.sh
│   │   ├── TEST-81-GENERATORS
│   │   │   └── meson.build
│   │   ├── TEST-82-SOFTREBOOT
│   │   │   └── meson.build
│   │   ├── TEST-83-BTRFS
│   │   │   └── meson.build
│   │   ├── TEST-84-STORAGETM
│   │   │   └── meson.build
│   │   ├── TEST-85-NETWORK
│   │   │   └── meson.build
│   │   ├── TEST-86-MULTI-PROFILE-UKI
│   │   │   └── meson.build
│   │   ├── TEST-87-AUX-UTILS-VM
│   │   │   └── meson.build
│   │   └── TEST-88-UPGRADE
│   │       └── meson.build
│   ├── journal-data
│   │   ├── journal-1.txt
│   │   └── journal-2.txt
│   ├── knot-data
│   │   ├── knot.conf
│   │   └── zones
│   │       ├── onlinesign.test.zone
│   │       ├── root.zone
│   │       ├── signed.test.zone
│   │       ├── test.zone
│   │       ├── unsigned.test.zone
│   │       └── untrusted.test.zone
│   ├── meson.build
│   ├── networkd-test.py
│   ├── rule-syntax-check.py
│   ├── run-unit-tests.py
│   ├── sd-script.py
│   ├── sys-script.py
│   ├── sysv-generator-test.py
│   ├── test-bcd
│   │   ├── corrupt.bcd.zst
│   │   ├── description-bad-type.bcd.zst
│   │   ├── description-empty.bcd.zst
│   │   ├── description-missing.bcd.zst
│   │   ├── description-too-small.bcd.zst
│   │   ├── displayorder-bad-name.bcd.zst
│   │   ├── displayorder-bad-size.bcd.zst
│   │   ├── displayorder-bad-type.bcd.zst
│   │   ├── empty.bcd.zst
│   │   └── win10.bcd.zst
│   ├── test-bootctl-json.sh
│   ├── test-compare-versions.sh
│   ├── test-execute
│   │   ├── exec-ambientcapabilities-dynuser.service
│   │   ├── exec-ambientcapabilities-merge-nfsnobody.service
│   │   ├── exec-ambientcapabilities-merge-nobody.service
│   │   ├── exec-ambientcapabilities-merge.service
│   │   ├── exec-ambientcapabilities-nfsnobody.service
│   │   ├── exec-ambientcapabilities-nobody.service
│   │   ├── exec-ambientcapabilities.service
│   │   ├── exec-basic.service
│   │   ├── exec-bindpaths.service
│   │   ├── exec-capabilityboundingset-invert.service
│   │   ├── exec-capabilityboundingset-merge.service
│   │   ├── exec-capabilityboundingset-reset.service
│   │   ├── exec-capabilityboundingset-simple.service
│   │   ├── exec-condition-failed.service
│   │   ├── exec-condition-skip.service
│   │   ├── exec-cpuaffinity1.service
│   │   ├── exec-cpuaffinity2.service
│   │   ├── exec-cpuaffinity3.service
│   │   ├── exec-credentials-dir-specifier.service
│   │   ├── exec-dynamicuser-fixeduser-adm.service
│   │   ├── exec-dynamicuser-fixeduser-games.service
│   │   ├── exec-dynamicuser-fixeduser-one-supplementarygroup.service
│   │   ├── exec-dynamicuser-fixeduser.service
│   │   ├── exec-dynamicuser-runtimedirectory1.service
│   │   ├── exec-dynamicuser-runtimedirectory2.service
│   │   ├── exec-dynamicuser-runtimedirectory3.service
│   │   ├── exec-dynamicuser-statedir-migrate-step1.service
│   │   ├── exec-dynamicuser-statedir-migrate-step2.service
│   │   ├── exec-dynamicuser-statedir.service
│   │   ├── exec-dynamicuser-supplementarygroups.service
│   │   ├── exec-environment-empty.service
│   │   ├── exec-environment-multiple.service
│   │   ├── exec-environment-no-substitute.service
│   │   ├── exec-environment.service
│   │   ├── exec-environmentfile.service
│   │   ├── exec-execsearchpath-environment-path-set.service
│   │   ├── exec-execsearchpath-environment.service
│   │   ├── exec-execsearchpath-environmentfile-set.service
│   │   ├── exec-execsearchpath-environmentfile.service
│   │   ├── exec-execsearchpath-passenvironment-set.service
│   │   ├── exec-execsearchpath-passenvironment.service
│   │   ├── exec-execsearchpath-unit-specifier.service
│   │   ├── exec-execsearchpath.service
│   │   ├── exec-group-nfsnobody.service
│   │   ├── exec-group-nobody.service
│   │   ├── exec-group-nogroup.service
│   │   ├── exec-group.service
│   │   ├── exec-ignoresigpipe-no.service
│   │   ├── exec-ignoresigpipe-yes.service
│   │   ├── exec-inaccessiblepaths-mount-propagation.service
│   │   ├── exec-inaccessiblepaths-sys.service
│   │   ├── exec-ioschedulingclass-best-effort.service
│   │   ├── exec-ioschedulingclass-idle.service
│   │   ├── exec-ioschedulingclass-none.service
│   │   ├── exec-ioschedulingclass-realtime.service
│   │   ├── exec-load-credential.service
│   │   ├── exec-mount-apivfs-no.service
│   │   ├── exec-networknamespacepath-privatemounts-no.service
│   │   ├── exec-networknamespacepath-privatemounts-yes.service
│   │   ├── exec-noexecpaths-simple.service
│   │   ├── exec-oomscoreadjust-negative.service
│   │   ├── exec-oomscoreadjust-positive.service
│   │   ├── exec-passenvironment-absent.service
│   │   ├── exec-passenvironment-empty.service
│   │   ├── exec-passenvironment-repeated.service
│   │   ├── exec-passenvironment.service
│   │   ├── exec-personality-aarch64.service
│   │   ├── exec-personality-loongarch64.service
│   │   ├── exec-personality-ppc64.service
│   │   ├── exec-personality-ppc64le.service
│   │   ├── exec-personality-s390.service
│   │   ├── exec-personality-s390x.service
│   │   ├── exec-personality-x86-64.service
│   │   ├── exec-personality-x86.service
│   │   ├── exec-privatedevices-bind.service
│   │   ├── exec-privatedevices-disabled-by-prefix.service
│   │   ├── exec-privatedevices-no-capability-mknod.service
│   │   ├── exec-privatedevices-no-capability-sys-rawio.service
│   │   ├── exec-privatedevices-no.service
│   │   ├── exec-privatedevices-yes-capability-mknod.service
│   │   ├── exec-privatedevices-yes-capability-sys-rawio.service
│   │   ├── exec-privatedevices-yes-with-group.service
│   │   ├── exec-privatedevices-yes.service
│   │   ├── exec-privatenetwork-yes-privatemounts-no.service
│   │   ├── exec-privatenetwork-yes-privatemounts-yes.service
│   │   ├── exec-privatetmp-disabled-by-prefix.service
│   │   ├── exec-privatetmp-disconnected-after-and-requires-for-var.service
│   │   ├── exec-privatetmp-disconnected-after-and-wants-for-var.service
│   │   ├── exec-privatetmp-disconnected-defaultdependencies-no.service
│   │   ├── exec-privatetmp-disconnected-nodefaultdeps-nor-sandboxing.service
│   │   ├── exec-privatetmp-disconnected-requires-mounts-for-var.service
│   │   ├── exec-privatetmp-disconnected-wants-mounts-for-var.service
│   │   ├── exec-privatetmp-disconnected.service
│   │   ├── exec-privatetmp-no.service
│   │   ├── exec-privatetmp-yes.service
│   │   ├── exec-protecthome-tmpfs-vs-protectsystem-strict.service
│   │   ├── exec-protectkernellogs-no-capabilities.service
│   │   ├── exec-protectkernellogs-yes-capabilities.service
│   │   ├── exec-protectkernelmodules-no-capabilities.service
│   │   ├── exec-protectkernelmodules-yes-capabilities.service
│   │   ├── exec-protectkernelmodules-yes-mount-propagation.service
│   │   ├── exec-readonlypaths-mount-propagation.service
│   │   ├── exec-readonlypaths-simple.service
│   │   ├── exec-readonlypaths-with-bindpaths.service
│   │   ├── exec-readonlypaths.service
│   │   ├── exec-readwritepaths-mount-propagation.service
│   │   ├── exec-restrictnamespaces-merge-all.service
│   │   ├── exec-restrictnamespaces-merge-and.service
│   │   ├── exec-restrictnamespaces-merge-or.service
│   │   ├── exec-restrictnamespaces-mnt-deny-list.service
│   │   ├── exec-restrictnamespaces-mnt.service
│   │   ├── exec-restrictnamespaces-no.service
│   │   ├── exec-restrictnamespaces-yes.service
│   │   ├── exec-runtimedirectory-mode.service
│   │   ├── exec-runtimedirectory-owner-nfsnobody.service
│   │   ├── exec-runtimedirectory-owner-nobody.service
│   │   ├── exec-runtimedirectory-owner-nogroup.service
│   │   ├── exec-runtimedirectory-owner.service
│   │   ├── exec-runtimedirectory.service
│   │   ├── exec-set-credential.service
│   │   ├── exec-specifier-interpolation.service
│   │   ├── exec-specifier-system.service
│   │   ├── exec-specifier-user.service
│   │   ├── exec-specifier.service
│   │   ├── exec-specifier@.service
│   │   ├── exec-standardinput-data.service
│   │   ├── exec-standardinput-file-cat.service
│   │   ├── exec-standardinput-file.service
│   │   ├── exec-standardoutput-append.service
│   │   ├── exec-standardoutput-file.service
│   │   ├── exec-standardoutput-truncate.service
│   │   ├── exec-supplementarygroups-multiple-groups-default-group-user.service
│   │   ├── exec-supplementarygroups-multiple-groups-withgid.service
│   │   ├── exec-supplementarygroups-multiple-groups-withuid.service
│   │   ├── exec-supplementarygroups-single-group-user.service
│   │   ├── exec-supplementarygroups-single-group.service
│   │   ├── exec-supplementarygroups.service
│   │   ├── exec-systemcallerrornumber-name.service
│   │   ├── exec-systemcallerrornumber-number.service
│   │   ├── exec-systemcallfilter-failing.service
│   │   ├── exec-systemcallfilter-failing2.service
│   │   ├── exec-systemcallfilter-failing3.service
│   │   ├── exec-systemcallfilter-nonewprivileges-bounding1.service
│   │   ├── exec-systemcallfilter-nonewprivileges-bounding2.service
│   │   ├── exec-systemcallfilter-nonewprivileges-protectclock.service
│   │   ├── exec-systemcallfilter-nonewprivileges.service
│   │   ├── exec-systemcallfilter-not-failing.service
│   │   ├── exec-systemcallfilter-not-failing2.service
│   │   ├── exec-systemcallfilter-not-failing3.service
│   │   ├── exec-systemcallfilter-override-error-action.service
│   │   ├── exec-systemcallfilter-override-error-action2.service
│   │   ├── exec-systemcallfilter-system-user-nfsnobody.service
│   │   ├── exec-systemcallfilter-system-user-nobody.service
│   │   ├── exec-systemcallfilter-system-user.service
│   │   ├── exec-systemcallfilter-with-errno-in-allow-list.service
│   │   ├── exec-systemcallfilter-with-errno-multi.service
│   │   ├── exec-systemcallfilter-with-errno-name.service
│   │   ├── exec-systemcallfilter-with-errno-number.service
│   │   ├── exec-systemcallfilter-writing-handoff-timestamp.service
│   │   ├── exec-temporaryfilesystem-options.service
│   │   ├── exec-temporaryfilesystem-ro.service
│   │   ├── exec-temporaryfilesystem-rw.service
│   │   ├── exec-temporaryfilesystem-usr.service
│   │   ├── exec-umask-0177.service
│   │   ├── exec-umask-default.service
│   │   ├── exec-umask-namespace.service
│   │   ├── exec-unsetenvironment.service
│   │   ├── exec-user-nfsnobody.service
│   │   ├── exec-user-nobody.service
│   │   ├── exec-user.service
│   │   ├── exec-workingdirectory-trailing-dot.service
│   │   └── exec-workingdirectory.service
│   ├── test-fstab-generator
│   │   ├── test-01-dev-nfs.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-01-dev-nfs.input
│   │   ├── test-02-dhcp.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-02-dhcp.input
│   │   ├── test-03-dhcp6.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-03-dhcp6.input
│   │   ├── test-04-nfs.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-04-nfs.input
│   │   ├── test-05-nfs4.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-05-nfs4.input
│   │   ├── test-06-ipv4.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-06-ipv4.input
│   │   ├── test-07-ipv6.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-07-ipv6.input
│   │   ├── test-08-implicit-nfs.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-08-implicit-nfs.input
│   │   ├── test-09-cifs.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-09-cifs.input
│   │   ├── test-10-iscsi.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-10-iscsi.input
│   │   ├── test-11-live.expected
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-11-live.input
│   │   ├── test-12-dev-sdx.expected
│   │   │   ├── initrd-root-device.target.d
│   │   │   │   └── 50-root-device.conf
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── sysroot.mount
│   │   │   └── systemd-fsck-root.service
│   │   ├── test-12-dev-sdx.input
│   │   ├── test-13-label.expected
│   │   │   ├── initrd-root-device.target.d
│   │   │   │   └── 50-root-device.conf
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── sysroot.mount
│   │   │   └── systemd-fsck-root.service
│   │   ├── test-13-label.input
│   │   ├── test-14-uuid.expected
│   │   │   ├── initrd-root-device.target.d
│   │   │   │   └── 50-root-device.conf
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── sysroot.mount
│   │   │   └── systemd-fsck-root.service
│   │   ├── test-14-uuid.input
│   │   ├── test-15-partuuid.expected
│   │   │   ├── initrd-root-device.target.d
│   │   │   │   └── 50-root-device.conf
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── sysroot.mount
│   │   │   └── systemd-fsck-root.service
│   │   ├── test-15-partuuid.input
│   │   ├── test-16-tmpfs.expected
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   └── sysroot.mount
│   │   ├── test-16-tmpfs.input
│   │   ├── test-17-initrd-sysroot.fstab.expected
│   │   │   ├── initrd-fs.target.requires
│   │   │   │   └── sysroot-usr.mount -> ../sysroot-usr.mount
│   │   │   ├── initrd-root-device.target.d
│   │   │   │   └── 50-root-device.conf
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   │   ├── sysroot.mount -> ../sysroot.mount
│   │   │   │   └── sysusr-usr.mount -> ../sysusr-usr.mount
│   │   │   ├── sysroot-usr.mount
│   │   │   ├── sysroot.mount
│   │   │   ├── systemd-fsck-root.service
│   │   │   └── sysusr-usr.mount
│   │   ├── test-17-initrd-sysroot.fstab.expected.sysroot
│   │   │   ├── local-fs.target.requires
│   │   │   │   ├── sysroot-usr.mount -> ../sysroot-usr.mount
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── local-fs.target.wants
│   │   │   │   └── systemd-remount-fs.service
│   │   │   ├── sysroot-usr.mount
│   │   │   └── sysroot.mount
│   │   ├── test-17-initrd-sysroot.fstab.input
│   │   ├── test-18-options.fstab.expected
│   │   │   ├── foo.service.requires
│   │   │   │   └── mnt-requiredby.mount -> ../mnt-requiredby.mount
│   │   │   ├── foo.service.wants
│   │   │   │   ├── mnt-wantedby-automount.automount -> ../mnt-wantedby-automount.automount
│   │   │   │   └── mnt-wantedby.mount -> ../mnt-wantedby.mount
│   │   │   ├── initrd-root-device.target.d
│   │   │   │   └── 50-root-device.conf
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── local-fs.target.d
│   │   │   │   └── 50-order-systemd-growfs@mnt-growfs.service.conf
│   │   │   ├── local-fs.target.requires
│   │   │   │   ├── mnt-after.mount -> ../mnt-after.mount
│   │   │   │   ├── mnt-automount1.automount -> ../mnt-automount1.automount
│   │   │   │   ├── mnt-before.mount -> ../mnt-before.mount
│   │   │   │   ├── mnt-growfs.mount -> ../mnt-growfs.mount
│   │   │   │   ├── mnt-mkfs.mount -> ../mnt-mkfs.mount
│   │   │   │   ├── mnt-pcrfs.mount -> ../mnt-pcrfs.mount
│   │   │   │   ├── mnt-reqmounts.mount -> ../mnt-reqmounts.mount
│   │   │   │   ├── mnt-requires.mount -> ../mnt-requires.mount
│   │   │   │   ├── mnt-rwonly.mount -> ../mnt-rwonly.mount
│   │   │   │   └── mnt-timeout.mount -> ../mnt-timeout.mount
│   │   │   ├── local-fs.target.wants
│   │   │   │   ├── mnt-automount2.automount -> ../mnt-automount2.automount
│   │   │   │   └── mnt-nofail.mount -> ../mnt-nofail.mount
│   │   │   ├── mnt-after.mount
│   │   │   ├── mnt-automount1.automount
│   │   │   ├── mnt-automount1.mount
│   │   │   ├── mnt-automount2.automount
│   │   │   ├── mnt-automount2.mount
│   │   │   ├── mnt-before.mount
│   │   │   ├── mnt-growfs.mount
│   │   │   ├── mnt-growfs.mount.wants
│   │   │   │   └── systemd-growfs@mnt-growfs.service
│   │   │   ├── mnt-mkfs.mount
│   │   │   ├── mnt-mkfs.mount.requires
│   │   │   │   └── systemd-makefs@dev-sdx12.service -> ../systemd-makefs@dev-sdx12.service
│   │   │   ├── mnt-noauto.mount
│   │   │   ├── mnt-nofail.mount
│   │   │   ├── mnt-pcrfs.mount
│   │   │   ├── mnt-reqmounts.mount
│   │   │   ├── mnt-requiredby.mount
│   │   │   ├── mnt-requires.mount
│   │   │   ├── mnt-rwonly.mount
│   │   │   ├── mnt-timeout.mount
│   │   │   ├── mnt-wantedby-automount.automount
│   │   │   ├── mnt-wantedby-automount.mount
│   │   │   ├── mnt-wantedby.mount
│   │   │   ├── sysroot.mount
│   │   │   ├── systemd-fsck-root.service
│   │   │   └── systemd-makefs@dev-sdx12.service
│   │   ├── test-18-options.fstab.expected.sysroot
│   │   │   ├── foo.service.requires
│   │   │   │   └── mnt-requiredby.mount -> ../mnt-requiredby.mount
│   │   │   ├── foo.service.wants
│   │   │   │   ├── mnt-wantedby-automount.automount -> ../mnt-wantedby-automount.automount
│   │   │   │   └── mnt-wantedby.mount -> ../mnt-wantedby.mount
│   │   │   ├── local-fs.target.d
│   │   │   │   └── 50-order-systemd-growfs@mnt-growfs.service.conf
│   │   │   ├── local-fs.target.requires
│   │   │   │   ├── mnt-after.mount -> ../mnt-after.mount
│   │   │   │   ├── mnt-automount1.automount -> ../mnt-automount1.automount
│   │   │   │   ├── mnt-before.mount -> ../mnt-before.mount
│   │   │   │   ├── mnt-growfs.mount -> ../mnt-growfs.mount
│   │   │   │   ├── mnt-mkfs.mount -> ../mnt-mkfs.mount
│   │   │   │   ├── mnt-pcrfs.mount -> ../mnt-pcrfs.mount
│   │   │   │   ├── mnt-reqmounts.mount -> ../mnt-reqmounts.mount
│   │   │   │   ├── mnt-requires.mount -> ../mnt-requires.mount
│   │   │   │   ├── mnt-rwonly.mount -> ../mnt-rwonly.mount
│   │   │   │   ├── mnt-timeout.mount -> ../mnt-timeout.mount
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── local-fs.target.wants
│   │   │   │   ├── mnt-automount2.automount -> ../mnt-automount2.automount
│   │   │   │   ├── mnt-nofail.mount -> ../mnt-nofail.mount
│   │   │   │   └── systemd-remount-fs.service
│   │   │   ├── mnt-after.mount
│   │   │   ├── mnt-automount1.automount
│   │   │   ├── mnt-automount1.mount
│   │   │   ├── mnt-automount2.automount
│   │   │   ├── mnt-automount2.mount
│   │   │   ├── mnt-before.mount
│   │   │   ├── mnt-growfs.mount
│   │   │   ├── mnt-growfs.mount.wants
│   │   │   │   └── systemd-growfs@mnt-growfs.service
│   │   │   ├── mnt-mkfs.mount
│   │   │   ├── mnt-mkfs.mount.requires
│   │   │   │   └── systemd-makefs@dev-sdx12.service -> ../systemd-makefs@dev-sdx12.service
│   │   │   ├── mnt-noauto.mount
│   │   │   ├── mnt-nofail.mount
│   │   │   ├── mnt-pcrfs.mount
│   │   │   ├── mnt-reqmounts.mount
│   │   │   ├── mnt-requiredby.mount
│   │   │   ├── mnt-requires.mount
│   │   │   ├── mnt-rwonly.mount
│   │   │   ├── mnt-timeout.mount
│   │   │   ├── mnt-wantedby-automount.automount
│   │   │   ├── mnt-wantedby-automount.mount
│   │   │   ├── mnt-wantedby.mount
│   │   │   ├── sysroot.mount
│   │   │   └── systemd-makefs@dev-sdx12.service
│   │   ├── test-18-options.fstab.input
│   │   ├── test-19-mounts-from-cmdline.expected
│   │   │   ├── hoge-without_fstype.mount
│   │   │   ├── hoge-without_options.mount
│   │   │   ├── hoge-withx20space.mount
│   │   │   ├── initrd-fs.target.requires
│   │   │   │   ├── sysroot-foo-also_in_initrd.mount -> ../sysroot-foo-also_in_initrd.mount
│   │   │   │   └── sysroot-usr.mount -> ../sysroot-usr.mount
│   │   │   ├── initrd-root-device.target.d
│   │   │   │   └── 50-root-device.conf
│   │   │   ├── initrd-root-fs.target.requires
│   │   │   │   └── sysroot.mount -> ../sysroot.mount
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   │   ├── sysroot.mount -> ../sysroot.mount
│   │   │   │   └── sysusr-usr.mount -> ../sysusr-usr.mount
│   │   │   ├── local-fs.target.requires
│   │   │   │   ├── hoge-without_fstype.mount -> ../hoge-without_fstype.mount
│   │   │   │   └── hoge-without_options.mount -> ../hoge-without_options.mount
│   │   │   ├── remote-fs.target.requires
│   │   │   │   └── hoge-withx20space.mount -> ../hoge-withx20space.mount
│   │   │   ├── sysroot-foo-also_in_initrd.mount
│   │   │   ├── sysroot-usr.mount
│   │   │   ├── sysroot.mount
│   │   │   ├── systemd-fsck-root.service
│   │   │   ├── systemd-fsck-usr.service
│   │   │   └── sysusr-usr.mount
│   │   ├── test-19-mounts-from-cmdline.expected.sysroot
│   │   │   ├── foo-also_in_initrd.mount
│   │   │   ├── foo-not_in_initrd.mount
│   │   │   ├── local-fs.target.requires
│   │   │   │   ├── foo-also_in_initrd.mount -> ../foo-also_in_initrd.mount
│   │   │   │   ├── foo-not_in_initrd.mount -> ../foo-not_in_initrd.mount
│   │   │   │   └── usr.mount -> ../usr.mount
│   │   │   └── usr.mount
│   │   ├── test-19-mounts-from-cmdline.input
│   │   ├── test-20-swap-from-cmdline.expected
│   │   │   ├── dev-sdy1.swap
│   │   │   ├── dev-sdy2.swap
│   │   │   ├── dev-sdy2.swap.requires
│   │   │   │   └── systemd-mkswap@dev-sdy2.service -> ../systemd-mkswap@dev-sdy2.service
│   │   │   ├── dev-sdy3.swap
│   │   │   ├── dev-sdy3.swap.requires
│   │   │   │   └── systemd-mkswap@dev-sdy3.service -> ../systemd-mkswap@dev-sdy3.service
│   │   │   ├── dev-sdy4.swap
│   │   │   ├── dev-sdy5.swap
│   │   │   ├── initrd-usr-fs.target.requires
│   │   │   │   └── sysroot.mount
│   │   │   ├── swap.target.requires
│   │   │   │   ├── dev-sdy1.swap -> ../dev-sdy1.swap
│   │   │   │   ├── dev-sdy2.swap -> ../dev-sdy2.swap
│   │   │   │   ├── dev-sdy4.swap -> ../dev-sdy4.swap
│   │   │   │   └── dev-sdy5.swap -> ../dev-sdy5.swap
│   │   │   ├── swap.target.wants
│   │   │   │   └── dev-sdy3.swap -> ../dev-sdy3.swap
│   │   │   ├── systemd-mkswap@dev-sdy2.service
│   │   │   └── systemd-mkswap@dev-sdy3.service
│   │   ├── test-20-swap-from-cmdline.expected.container
│   │   │   └── initrd-usr-fs.target.requires
│   │   │       └── sysroot.mount
│   │   ├── test-20-swap-from-cmdline.expected.sysroot
│   │   │   ├── dev-sdy5.swap
│   │   │   ├── dev-sdy6.swap
│   │   │   └── swap.target.requires
│   │   │       ├── dev-sdy5.swap -> ../dev-sdy5.swap
│   │   │       └── dev-sdy6.swap -> ../dev-sdy6.swap
│   │   └── test-20-swap-from-cmdline.input
│   ├── test-fstab-generator.sh
│   ├── test-journals
│   │   ├── afl-corrupted-journals.tar.zst
│   │   ├── corrupted
│   │   │   ├── id:000000,sig:06,src:000711,time:110015157,execs:33104794,op:MOpt_havoc,rep:2.zst
│   │   │   └── id:000000,src:000031,time:210669947,execs:34191940,op:havoc,rep:32.zst
│   │   └── no-rtc
│   │       ├── system.journal.zst
│   │       ├── system@0005ebbfd42fc981-39a8842ec948769a.journal~.zst
│   │       ├── system@0005ebbfd4346b9f-43185b46162d9fa5.journal~.zst
│   │       ├── system@0005ebbfd4385848-2e5dff5354ab9bcf.journal~.zst
│   │       ├── user-1000.journal.zst
│   │       ├── user-1000@0005ebbfd660bcbe-dbef2eee11f4b575.journal~.zst
│   │       └── user-1000@0005ebbfe89faec4-a5e890e7b00bedd1.journal~.zst
│   ├── test-keymap-util
│   │   └── kbd-model-map -> ../../src/locale/kbd-model-map
│   ├── test-network
│   │   ├── conf
│   │   │   ├── 00-debug-net.rules
│   │   │   ├── 10-dhcp-client-id-duid.conf
│   │   │   ├── 10-dhcp-client-id-mac.conf
│   │   │   ├── 10-dropin-test.netdev
│   │   │   ├── 10-dropin-test.netdev.d
│   │   │   │   ├── mac.conf
│   │   │   │   └── name.conf
│   │   │   ├── 11-dummy-mtu.netdev
│   │   │   ├── 11-dummy-unmanaged.link
│   │   │   ├── 11-dummy.netdev
│   │   │   ├── 11-dummy.network
│   │   │   ├── 11-test-unit-file.link
│   │   │   ├── 11-test-unit-file.link.d
│   │   │   │   └── dropin.conf
│   │   │   ├── 11-test-unit-file.netdev
│   │   │   ├── 11-test-unit-file.netdev.d
│   │   │   │   └── dropin.conf
│   │   │   ├── 11-test-unit-file.network
│   │   │   ├── 11-test-unit-file.network.d
│   │   │   │   └── dropin.conf
│   │   │   ├── 12-dummy-altname.link
│   │   │   ├── 12-dummy-mac.netdev
│   │   │   ├── 12-dummy-match-altname.network
│   │   │   ├── 12-dummy-match-mac-01.network
│   │   │   ├── 12-dummy-match-mac-02.network
│   │   │   ├── 12-dummy-match-renamed.network
│   │   │   ├── 12-dummy-mtu.link
│   │   │   ├── 12-dummy-mtu.netdev
│   │   │   ├── 12-dummy-no-address.network
│   │   │   ├── 12-dummy-rename-to-altname.link
│   │   │   ├── 12-dummy.link
│   │   │   ├── 12-dummy.netdev
│   │   │   ├── 12-dummy.network
│   │   │   ├── 12-dummy.network.d
│   │   │   │   ├── ipv6-mtu-1400.conf
│   │   │   │   ├── ipv6-mtu-1550.conf
│   │   │   │   └── mtu.conf
│   │   │   ├── 13-dummy.netdev
│   │   │   ├── 13-not-match-udev-property.network
│   │   │   ├── 14-dummy.netdev
│   │   │   ├── 14-match-udev-property.network
│   │   │   ├── 15-name-conflict-test.netdev
│   │   │   ├── 21-bond-802.3ad.netdev
│   │   │   ├── 21-bond-802.3ad.network
│   │   │   ├── 21-dummy-bond-slave.network
│   │   │   ├── 21-macvlan.netdev
│   │   │   ├── 21-macvtap.netdev
│   │   │   ├── 21-vlan-on-bond.netdev
│   │   │   ├── 21-vlan-on-bond.network
│   │   │   ├── 21-vlan-test1.network
│   │   │   ├── 21-vlan-test1.network.d
│   │   │   │   └── override.conf
│   │   │   ├── 21-vlan.netdev
│   │   │   ├── 21-vlan.netdev.d
│   │   │   │   └── override.conf
│   │   │   ├── 21-vlan.network
│   │   │   ├── 23-active-slave.network
│   │   │   ├── 23-bond199.network
│   │   │   ├── 23-emit-lldp.network
│   │   │   ├── 23-keep-master.network
│   │   │   ├── 23-primary-slave.network
│   │   │   ├── 24-keep-configuration-static.network
│   │   │   ├── 24-keep-configuration-yes.network
│   │   │   ├── 24-lldp.network
│   │   │   ├── 24-rps-cpu-disable.link
│   │   │   ├── 24-rps-cpu-empty.link
│   │   │   ├── 24-rps-cpu-invalid.link
│   │   │   ├── 24-search-domain.network
│   │   │   ├── 25-6rd-tunnel.netdev
│   │   │   ├── 25-6rd.network
│   │   │   ├── 25-activation-policy.network
│   │   │   ├── 25-activation-policy.network.d
│   │   │   │   ├── always-down.conf
│   │   │   │   ├── always-up.conf
│   │   │   │   ├── bound.conf
│   │   │   │   ├── down.conf
│   │   │   │   ├── manual.conf
│   │   │   │   ├── required-no.conf
│   │   │   │   ├── required-yes.conf
│   │   │   │   └── up.conf
│   │   │   ├── 25-address-ipv4acd-veth99.network
│   │   │   ├── 25-address-ipv4acd-veth99.network.d
│   │   │   │   └── conflict-address.conf
│   │   │   ├── 25-address-link-section.network
│   │   │   ├── 25-address-peer-ipv4.network
│   │   │   ├── 25-address-static.network
│   │   │   ├── 25-address-static.network.d
│   │   │   │   ├── 10-many-address.conf
│   │   │   │   ├── 10-override.conf
│   │   │   │   └── 20-clear-addresses.conf
│   │   │   ├── 25-agent-bridge-port.network
│   │   │   ├── 25-agent-bridge.netdev
│   │   │   ├── 25-agent-bridge.network
│   │   │   ├── 25-agent-client-peer.network
│   │   │   ├── 25-agent-client.network
│   │   │   ├── 25-agent-server-peer.network
│   │   │   ├── 25-agent-server.network
│   │   │   ├── 25-agent-veth-client.netdev
│   │   │   ├── 25-agent-veth-server.netdev
│   │   │   ├── 25-bareudp.netdev
│   │   │   ├── 25-batadv.netdev
│   │   │   ├── 25-bind-carrier.network
│   │   │   ├── 25-bond-active-backup-slave.netdev
│   │   │   ├── 25-bond-balanced-tlb.netdev
│   │   │   ├── 25-bond-property.netdev
│   │   │   ├── 25-bond-slave.network
│   │   │   ├── 25-bond.netdev
│   │   │   ├── 25-bond99.network
│   │   │   ├── 25-bootp-client.network
│   │   │   ├── 25-bridge-configure-without-carrier.network
│   │   │   ├── 25-bridge.netdev
│   │   │   ├── 25-bridge.network
│   │   │   ├── 25-bridge99-ignore-carrier-loss.network
│   │   │   ├── 25-bridge99.network
│   │   │   ├── 25-default.link
│   │   │   ├── 25-dhcp-client-allow-list.network
│   │   │   ├── 25-dhcp-client-allow-list.network.d
│   │   │   │   ├── 00-allow-list.conf
│   │   │   │   └── 10-deny-list.conf
│   │   │   ├── 25-dhcp-client-anonymize.network
│   │   │   ├── 25-dhcp-client-gateway-onlink-implicit.network
│   │   │   ├── 25-dhcp-client-ipv4-only.network
│   │   │   ├── 25-dhcp-client-ipv4-use-routes-use-gateway.network
│   │   │   ├── 25-dhcp-client-ipv4-use-routes-use-gateway.network.d
│   │   │   │   ├── use-dns-and-ntp-routes-False.conf
│   │   │   │   ├── use-dns-and-ntp-routes-True.conf
│   │   │   │   ├── use-gateway-False.conf
│   │   │   │   ├── use-gateway-True.conf
│   │   │   │   ├── use-routes-False.conf
│   │   │   │   └── use-routes-True.conf
│   │   │   ├── 25-dhcp-client-ipv6-only-custom-client-identifier.network
│   │   │   ├── 25-dhcp-client-ipv6-only-mode.network
│   │   │   ├── 25-dhcp-client-ipv6-only.network
│   │   │   ├── 25-dhcp-client-keep-configuration-dynamic-on-stop.network
│   │   │   ├── 25-dhcp-client-keep-configuration-dynamic.network
│   │   │   ├── 25-dhcp-client-static-lease.network
│   │   │   ├── 25-dhcp-client-timezone-router.network
│   │   │   ├── 25-dhcp-client-use-dns-ipv4-and-ra.network
│   │   │   ├── 25-dhcp-client-use-dns-ipv4.network
│   │   │   ├── 25-dhcp-client-use-dns-no.network
│   │   │   ├── 25-dhcp-client-use-dns-yes.network
│   │   │   ├── 25-dhcp-client-vrf.network
│   │   │   ├── 25-dhcp-client-with-ipv4ll.network
│   │   │   ├── 25-dhcp-client.network
│   │   │   ├── 25-dhcp-pd-downstream-dummy97.network
│   │   │   ├── 25-dhcp-pd-downstream-dummy98.network
│   │   │   ├── 25-dhcp-pd-downstream-dummy99.network
│   │   │   ├── 25-dhcp-pd-downstream-test1.network
│   │   │   ├── 25-dhcp-pd-downstream-veth97-peer.network
│   │   │   ├── 25-dhcp-pd-downstream-veth97.network
│   │   │   ├── 25-dhcp-pd-downstream-veth98-peer.network
│   │   │   ├── 25-dhcp-pd-downstream-veth98.network
│   │   │   ├── 25-dhcp-server-downstream.network
│   │   │   ├── 25-dhcp-server-ipv6-only-mode.network
│   │   │   ├── 25-dhcp-server-null-server-address.network
│   │   │   ├── 25-dhcp-server-static-lease.network
│   │   │   ├── 25-dhcp-server-timezone-router.network
│   │   │   ├── 25-dhcp-server-uplink.network
│   │   │   ├── 25-dhcp-server-veth-peer.network
│   │   │   ├── 25-dhcp-server.network
│   │   │   ├── 25-dhcp4-6rd-server.network
│   │   │   ├── 25-dhcp4-6rd-upstream.network
│   │   │   ├── 25-dhcp6pd-server.network
│   │   │   ├── 25-dhcp6pd-upstream-no-address.network
│   │   │   ├── 25-dhcp6pd-upstream-no-assign.network
│   │   │   ├── 25-dhcp6pd-upstream.network
│   │   │   ├── 25-dummy.netdev
│   │   │   ├── 25-dummy.network
│   │   │   ├── 25-erspan.network
│   │   │   ├── 25-erspan0-tunnel-local-any.netdev
│   │   │   ├── 25-erspan0-tunnel.netdev
│   │   │   ├── 25-erspan1-tunnel-local-any.netdev
│   │   │   ├── 25-erspan1-tunnel.netdev
│   │   │   ├── 25-erspan2-tunnel-local-any.netdev
│   │   │   ├── 25-erspan2-tunnel.netdev
│   │   │   ├── 25-fibrule-invert.network
│   │   │   ├── 25-fibrule-l3mdev.network
│   │   │   ├── 25-fibrule-port-range.network
│   │   │   ├── 25-fibrule-uidrange.network
│   │   │   ├── 25-fou-gre.netdev
│   │   │   ├── 25-fou-gretap.netdev
│   │   │   ├── 25-fou-ipip.netdev
│   │   │   ├── 25-fou-ipproto-gre.netdev
│   │   │   ├── 25-fou-ipproto-ipip.netdev
│   │   │   ├── 25-fou-sit.netdev
│   │   │   ├── 25-gateway-next-static.network
│   │   │   ├── 25-gateway-static.network
│   │   │   ├── 25-geneve.netdev
│   │   │   ├── 25-global-ipv6-privacy-extensions.conf
│   │   │   ├── 25-gre-tunnel-any-any.netdev
│   │   │   ├── 25-gre-tunnel-local-any.netdev
│   │   │   ├── 25-gre-tunnel-remote-any.netdev
│   │   │   ├── 25-gre-tunnel.netdev
│   │   │   ├── 25-gretap-tunnel-local-any.netdev
│   │   │   ├── 25-gretap-tunnel.netdev
│   │   │   ├── 25-gretap.network
│   │   │   ├── 25-gretun.network
│   │   │   ├── 25-hsr.netdev
│   │   │   ├── 25-hsr.network
│   │   │   ├── 25-ifb.netdev
│   │   │   ├── 25-ip6gre-tunnel-any-any.netdev
│   │   │   ├── 25-ip6gre-tunnel-local-any.netdev
│   │   │   ├── 25-ip6gre-tunnel-remote-any.netdev
│   │   │   ├── 25-ip6gre-tunnel.netdev
│   │   │   ├── 25-ip6gretap-tunnel-local-any.netdev
│   │   │   ├── 25-ip6gretap-tunnel.netdev
│   │   │   ├── 25-ip6gretap.network
│   │   │   ├── 25-ip6gretun.network
│   │   │   ├── 25-ip6tnl-slaac.network
│   │   │   ├── 25-ip6tnl-tunnel-external.netdev
│   │   │   ├── 25-ip6tnl-tunnel-local-any.netdev
│   │   │   ├── 25-ip6tnl-tunnel-local-slaac.netdev
│   │   │   ├── 25-ip6tnl-tunnel-local-slaac.network
│   │   │   ├── 25-ip6tnl-tunnel-remote-any.netdev
│   │   │   ├── 25-ip6tnl-tunnel.netdev
│   │   │   ├── 25-ip6tnl.network
│   │   │   ├── 25-ipip-tunnel-any-any.netdev
│   │   │   ├── 25-ipip-tunnel-independent-loopback.netdev
│   │   │   ├── 25-ipip-tunnel-independent.netdev
│   │   │   ├── 25-ipip-tunnel-local-any.netdev
│   │   │   ├── 25-ipip-tunnel-remote-any.netdev
│   │   │   ├── 25-ipip-tunnel.netdev
│   │   │   ├── 25-ipip.network
│   │   │   ├── 25-ipv6-address-label-section.network
│   │   │   ├── 25-ipv6-neigh-retrans-time-0s.network
│   │   │   ├── 25-ipv6-neigh-retrans-time-3s.network
│   │   │   ├── 25-ipv6-neigh-retrans-time-4s.network
│   │   │   ├── 25-ipv6-neigh-retrans-time-infinity.network
│   │   │   ├── 25-ipv6-neigh-retrans-time-invalid.network
│   │   │   ├── 25-ipv6-neigh-retrans-time-toobig.network
│   │   │   ├── 25-ipv6-prefix-veth-static-route.network
│   │   │   ├── 25-ipv6-prefix-veth-token-prefixstable-without-address.network
│   │   │   ├── 25-ipv6-prefix-veth-token-prefixstable.network
│   │   │   ├── 25-ipv6-prefix-veth-token-static.network
│   │   │   ├── 25-ipv6-prefix-veth.network
│   │   │   ├── 25-ipv6-prefix.network
│   │   │   ├── 25-ipv6-proxy-ndp.network
│   │   │   ├── 25-ipv6ra-prefix-client-deny-list.network
│   │   │   ├── 25-ipv6ra-prefix-client.network
│   │   │   ├── 25-ipv6ra-prefix.network
│   │   │   ├── 25-ipv6ra-uplink.network
│   │   │   ├── 25-ipvlan.netdev
│   │   │   ├── 25-ipvlan.network
│   │   │   ├── 25-ipvtap.netdev
│   │   │   ├── 25-ipvtap.network
│   │   │   ├── 25-isatap-tunnel.netdev
│   │   │   ├── 25-isatap.network
│   │   │   ├── 25-l2tp-dummy.network
│   │   │   ├── 25-l2tp-ip.netdev
│   │   │   ├── 25-l2tp-udp.netdev
│   │   │   ├── 25-l2tp.network
│   │   │   ├── 25-link-local-addressing-no.network
│   │   │   ├── 25-link-local-addressing-yes.network
│   │   │   ├── 25-link-section-unmanaged.network
│   │   │   ├── 25-macsec.key
│   │   │   ├── 25-macsec.netdev
│   │   │   ├── 25-macsec.network
│   │   │   ├── 25-macvlan.network
│   │   │   ├── 25-macvtap.network
│   │   │   ├── 25-neighbor-dummy.network
│   │   │   ├── 25-neighbor-dummy.network.d
│   │   │   │   ├── 10-step1.conf
│   │   │   │   ├── 10-step2.conf
│   │   │   │   └── 10-step3.conf
│   │   │   ├── 25-neighbor-ip.network
│   │   │   ├── 25-neighbor-ipv6.network
│   │   │   ├── 25-netdevsim.link
│   │   │   ├── 25-nexthop-1.network
│   │   │   ├── 25-nexthop-2.network
│   │   │   ├── 25-nexthop-dummy-1.network
│   │   │   ├── 25-nexthop-dummy-2.network
│   │   │   ├── 25-nexthop-nothing.network
│   │   │   ├── 25-nexthop-test1.network
│   │   │   ├── 25-nlmon.netdev
│   │   │   ├── 25-prefix-route-with-vrf.network
│   │   │   ├── 25-prefix-route-without-vrf.network
│   │   │   ├── 25-qdisc-cake.network
│   │   │   ├── 25-qdisc-clsact.network
│   │   │   ├── 25-qdisc-codel.network
│   │   │   ├── 25-qdisc-drr.network
│   │   │   ├── 25-qdisc-ets.network
│   │   │   ├── 25-qdisc-fq_codel.network
│   │   │   ├── 25-qdisc-fq_pie.network
│   │   │   ├── 25-qdisc-fq.network
│   │   │   ├── 25-qdisc-gred.network
│   │   │   ├── 25-qdisc-hhf.network
│   │   │   ├── 25-qdisc-htb-fifo.network
│   │   │   ├── 25-qdisc-ingress.network
│   │   │   ├── 25-qdisc-mq.network
│   │   │   ├── 25-qdisc-multiq.network
│   │   │   ├── 25-qdisc-netem-compat.network
│   │   │   ├── 25-qdisc-netem.network
│   │   │   ├── 25-qdisc-pie.network
│   │   │   ├── 25-qdisc-qfq.network
│   │   │   ├── 25-qdisc-sfb.network
│   │   │   ├── 25-qdisc-sfq.network
│   │   │   ├── 25-qdisc-tbf.network
│   │   │   ├── 25-qdisc-teql.network
│   │   │   ├── 25-route-congctl.network
│   │   │   ├── 25-route-ipv6-src.network
│   │   │   ├── 25-route-preferred-source.network
│   │   │   ├── 25-route-static-issue-35047.network
│   │   │   ├── 25-route-static-issue-35047.network.d
│   │   │   │   ├── step1.conf
│   │   │   │   └── step2.conf
│   │   │   ├── 25-route-static-issue-37714.network
│   │   │   ├── 25-route-static-test1.network
│   │   │   ├── 25-route-static.network
│   │   │   ├── 25-route-via-ipv6.network
│   │   │   ├── 25-route-vrf.network
│   │   │   ├── 25-routing-policy-rule-dummy98.network
│   │   │   ├── 25-routing-policy-rule-manual.network
│   │   │   ├── 25-routing-policy-rule-reconfigure1.network
│   │   │   ├── 25-routing-policy-rule-reconfigure2.network
│   │   │   ├── 25-routing-policy-rule-test1.network
│   │   │   ├── 25-rps-cpu-0-1.link
│   │   │   ├── 25-rps-cpu-0-empty.link
│   │   │   ├── 25-rps-cpu-0-invalid.link
│   │   │   ├── 25-rps-cpu-0.link
│   │   │   ├── 25-rps-cpu-1.link
│   │   │   ├── 25-rps-cpu-all.link
│   │   │   ├── 25-rps-cpu-multi.link
│   │   │   ├── 25-sit-dhcp4.netdev
│   │   │   ├── 25-sit-dhcp4.network
│   │   │   ├── 25-sit-tunnel-any-any.netdev
│   │   │   ├── 25-sit-tunnel-local-any.netdev
│   │   │   ├── 25-sit-tunnel-remote-any.netdev
│   │   │   ├── 25-sit-tunnel.netdev
│   │   │   ├── 25-sit.network
│   │   │   ├── 25-sriov-udev.network
│   │   │   ├── 25-sriov.link
│   │   │   ├── 25-sriov.network
│   │   │   ├── 25-state-file-tests.network
│   │   │   ├── 25-sysctl-disable-ipv6.network
│   │   │   ├── 25-sysctl-mpls.network
│   │   │   ├── 25-sysctl.network
│   │   │   ├── 25-sysctl.network.d
│   │   │   │   └── 25-ipv6-privacy-extensions.conf
│   │   │   ├── 25-tap.netdev
│   │   │   ├── 25-test1.network
│   │   │   ├── 25-test1.network.d
│   │   │   │   ├── configure-without-carrier.conf
│   │   │   │   └── ignore-carrier-loss-no.conf
│   │   │   ├── 25-tun.netdev
│   │   │   ├── 25-tunnel-any-any.network
│   │   │   ├── 25-tunnel-local-any.network
│   │   │   ├── 25-tunnel-remote-any.network
│   │   │   ├── 25-tunnel.network
│   │   │   ├── 25-vcan.netdev
│   │   │   ├── 25-vcan98.netdev
│   │   │   ├── 25-vcan98.network
│   │   │   ├── 25-veth-bridge-captive.network
│   │   │   ├── 25-veth-bridge.network
│   │   │   ├── 25-veth-client-captive.network
│   │   │   ├── 25-veth-client.netdev
│   │   │   ├── 25-veth-client.network
│   │   │   ├── 25-veth-downstream-veth97.netdev
│   │   │   ├── 25-veth-downstream-veth98.netdev
│   │   │   ├── 25-veth-mtu.netdev
│   │   │   ├── 25-veth-peer-no-address.network
│   │   │   ├── 25-veth-peer.network
│   │   │   ├── 25-veth-router-captive.netdev
│   │   │   ├── 25-veth-router-captive.network
│   │   │   ├── 25-veth-router-high.netdev
│   │   │   ├── 25-veth-router-high.network
│   │   │   ├── 25-veth-router-hop-limit.network
│   │   │   ├── 25-veth-router-low.netdev
│   │   │   ├── 25-veth-router-low.network
│   │   │   ├── 25-veth-router.netdev
│   │   │   ├── 25-veth.netdev
│   │   │   ├── 25-vrf.netdev
│   │   │   ├── 25-vrf.network
│   │   │   ├── 25-vti-tunnel-any-any.netdev
│   │   │   ├── 25-vti-tunnel-local-any.netdev
│   │   │   ├── 25-vti-tunnel-remote-any.netdev
│   │   │   ├── 25-vti-tunnel.netdev
│   │   │   ├── 25-vti.network
│   │   │   ├── 25-vti6-tunnel-local-any.netdev
│   │   │   ├── 25-vti6-tunnel-remote-any.netdev
│   │   │   ├── 25-vti6-tunnel.netdev
│   │   │   ├── 25-vti6.network
│   │   │   ├── 25-vxcan.netdev
│   │   │   ├── 25-vxlan-external.netdev
│   │   │   ├── 25-vxlan-external.network
│   │   │   ├── 25-vxlan-independent.netdev
│   │   │   ├── 25-vxlan-ipv6.netdev
│   │   │   ├── 25-vxlan-ipv6.network
│   │   │   ├── 25-vxlan-local-slaac.netdev
│   │   │   ├── 25-vxlan-local-slaac.network
│   │   │   ├── 25-vxlan-test1.network
│   │   │   ├── 25-vxlan-veth99.network
│   │   │   ├── 25-vxlan.netdev
│   │   │   ├── 25-vxlan.network
│   │   │   ├── 25-wireguard-23-peers.netdev
│   │   │   ├── 25-wireguard-23-peers.network
│   │   │   ├── 25-wireguard-endpoint-peer0-cred.txt
│   │   │   ├── 25-wireguard-no-peer-private-key-cred.txt
│   │   │   ├── 25-wireguard-no-peer.netdev
│   │   │   ├── 25-wireguard-no-peer.network
│   │   │   ├── 25-wireguard-preshared-key-peer2-cred.txt
│   │   │   ├── 25-wireguard-preshared-key.txt
│   │   │   ├── 25-wireguard-private-key.txt
│   │   │   ├── 25-wireguard-public-key.txt
│   │   │   ├── 25-wireguard.netdev
│   │   │   ├── 25-wireguard.netdev.d
│   │   │   │   ├── peer.conf
│   │   │   │   ├── peer1.conf
│   │   │   │   ├── peer2.conf
│   │   │   │   └── private-key.conf
│   │   │   ├── 25-wireguard.network
│   │   │   ├── 25-xfrm-independent.netdev
│   │   │   ├── 25-xfrm.netdev
│   │   │   ├── 25-xfrm.network
│   │   │   ├── 26-bridge-configure-without-carrier.network
│   │   │   ├── 26-bridge-issue-20373.netdev
│   │   │   ├── 26-bridge-mac-master.network
│   │   │   ├── 26-bridge-mac-slave.network
│   │   │   ├── 26-bridge-mac.link
│   │   │   ├── 26-bridge-mac.netdev
│   │   │   ├── 26-bridge-mdb-master.network
│   │   │   ├── 26-bridge-mdb-slave.network
│   │   │   ├── 26-bridge-slave-interface-1.network
│   │   │   ├── 26-bridge-slave-interface-2.network
│   │   │   ├── 26-bridge-vlan-master-issue-20373.network
│   │   │   ├── 26-bridge-vlan-master.network
│   │   │   ├── 26-bridge-vlan-master.network.d
│   │   │   │   ├── 10-override.conf
│   │   │   │   ├── 20-override.conf
│   │   │   │   └── 30-override.conf
│   │   │   ├── 26-bridge-vlan-slave-issue-20373.network
│   │   │   ├── 26-bridge-vlan-slave.network
│   │   │   ├── 26-bridge-vlan-slave.network.d
│   │   │   │   ├── 10-override.conf
│   │   │   │   ├── 20-override.conf
│   │   │   │   └── 30-override.conf
│   │   │   ├── 26-bridge-vlan-tunnel.network
│   │   │   ├── 26-bridge.netdev
│   │   │   ├── 26-link-local-addressing-ipv6.network
│   │   │   ├── 26-macsec.network
│   │   │   ├── 26-netdev-link-local-addressing-yes.network
│   │   │   ├── 80-6rd-tunnel.network
│   │   │   ├── 85-static-ipv6.network
│   │   │   ├── 85-unmanaged.link
│   │   │   ├── isc-dhcpd-dhcp6pd-no-range.conf
│   │   │   ├── isc-dhcpd-dhcp6pd.conf
│   │   │   ├── networkd-address-label.conf
│   │   │   ├── networkd-manage-foreign-nexthops-no.conf
│   │   │   ├── networkd-manage-foreign-routes-no.conf
│   │   │   ├── networkd-manage-foreign-rules-no.conf
│   │   │   ├── persist-leases-no.conf
│   │   │   ├── persist-leases-runtime.conf
│   │   │   └── radvd
│   │   │       └── captive-portal.conf
│   │   └── systemd-networkd-tests.py
│   ├── test-network-generator-conversion
│   │   ├── test-01-dhcp.expected
│   │   │   └── 71-default.network
│   │   ├── test-01-dhcp.input
│   │   ├── test-02-bridge.expected
│   │   │   ├── 70-bridge99.netdev
│   │   │   ├── 70-bridge99.network
│   │   │   ├── 70-eth0.network
│   │   │   └── 70-eth1.network
│   │   ├── test-02-bridge.input
│   │   ├── test-03-issue-14319.expected
│   │   │   └── 70-enp3s0.network
│   │   └── test-03-issue-14319.input
│   ├── test-network-generator-conversion.sh
│   ├── test-path
│   │   ├── basic.target
│   │   ├── path-changed.path
│   │   ├── path-changed.service
│   │   ├── path-directorynotempty.path
│   │   ├── path-directorynotempty.service
│   │   ├── path-exists.path
│   │   ├── path-exists.service
│   │   ├── path-existsglob.path
│   │   ├── path-existsglob.service
│   │   ├── path-makedirectory.path
│   │   ├── path-makedirectory.service
│   │   ├── path-modified.path
│   │   ├── path-modified.service
│   │   ├── path-mycustomunit.service
│   │   ├── path-unit.path
│   │   ├── paths.target
│   │   └── sysinit.target
│   ├── test-path-util
│   │   └── script.sh
│   ├── test-resolve
│   │   ├── _443._tcp.fedoraproject.org.pkts
│   │   ├── _openpgpkey.fedoraproject.org.pkts
│   │   ├── com~20200417.pkts
│   │   ├── fake-caa.pkts
│   │   ├── fedoraproject.org.pkts
│   │   ├── gandi.net.pkts
│   │   ├── google.com~20160131.pkts
│   │   ├── google.com~20200417.pkts
│   │   ├── kyhwana.org.pkts
│   │   ├── michigan.gov~20200417.pkts
│   │   ├── org~20200417.pkts
│   │   ├── root.pkts
│   │   ├── selfsigned.cert
│   │   ├── selfsigned.key
│   │   ├── sw1a1aa-sw1a2aa-sw1a2ab-sw1a2ac.find.me.uk.pkts
│   │   ├── teamits.com.pkts
│   │   ├── vdwaa.nl~20200417.pkts
│   │   └── zbyszek@fedoraproject.org.pkts
│   ├── test-rpm-macros.sh
│   ├── test-shutdown.py
│   ├── test-systemctl-enable.sh
│   ├── test-systemd-tmpfiles.py
│   ├── test-sysusers
│   │   ├── inline.expected-group
│   │   ├── inline.expected-passwd
│   │   ├── test-00-basic.expected-group
│   │   ├── test-00-basic.expected-passwd
│   │   ├── test-00-basic.input
│   │   ├── test-1.expected-group
│   │   ├── test-1.expected-passwd
│   │   ├── test-1.input
│   │   ├── test-10.expected-group
│   │   ├── test-10.expected-passwd
│   │   ├── test-10.input
│   │   ├── test-11.expected-group
│   │   ├── test-11.expected-passwd
│   │   ├── test-11.initial-group
│   │   ├── test-11.initial-passwd
│   │   ├── test-11.input
│   │   ├── test-12.expected-group
│   │   ├── test-12.expected-passwd
│   │   ├── test-12.initial-group
│   │   ├── test-12.initial-passwd
│   │   ├── test-12.input
│   │   ├── test-13.expected-group
│   │   ├── test-13.expected-passwd
│   │   ├── test-13.input
│   │   ├── test-14.expected-group
│   │   ├── test-14.expected-passwd
│   │   ├── test-14.initial-group
│   │   ├── test-14.input
│   │   ├── test-15.expected-group
│   │   ├── test-15.expected-passwd
│   │   ├── test-15.initial-passwd
│   │   ├── test-15.input
│   │   ├── test-16.expected-group
│   │   ├── test-16.expected-passwd
│   │   ├── test-16.input
│   │   ├── test-2.expected-group
│   │   ├── test-2.expected-passwd
│   │   ├── test-2.input
│   │   ├── test-3.expected-group
│   │   ├── test-3.expected-passwd
│   │   ├── test-3.input
│   │   ├── test-4.expected-group
│   │   ├── test-4.expected-passwd
│   │   ├── test-4.input
│   │   ├── test-5.expected-group
│   │   ├── test-5.expected-passwd
│   │   ├── test-5.input
│   │   ├── test-6.expected-group
│   │   ├── test-6.expected-passwd
│   │   ├── test-6.input
│   │   ├── test-7.expected-group
│   │   ├── test-7.expected-passwd
│   │   ├── test-7.input
│   │   ├── test-8.expected-group
│   │   ├── test-8.expected-passwd
│   │   ├── test-8.input
│   │   ├── test-9.expected-group
│   │   ├── test-9.expected-passwd
│   │   ├── test-9.input
│   │   ├── unhappy-1.expected-err
│   │   ├── unhappy-1.input
│   │   ├── unhappy-2.expected-err
│   │   ├── unhappy-2.input
│   │   ├── unhappy-3.expected-err
│   │   └── unhappy-3.input
│   ├── test-sysusers.sh.in
│   ├── test-udev.py
│   ├── test-umount
│   │   ├── empty.mountinfo
│   │   ├── example.swaps
│   │   ├── garbled.mountinfo
│   │   └── rhbug-1554943.mountinfo
│   ├── test.service.in
│   ├── testdata -> .
│   ├── udev-dmi-memory-id-test.sh
│   └── units
│       ├── a-conj.service
│       ├── a.service
│       ├── autorelabel.service
│       ├── b.service
│       ├── basic.target
│       ├── c.service
│       ├── d.service
│       ├── daughter.service
│       ├── delegated_cgroup_filtering_payload_child.sh
│       ├── delegated_cgroup_filtering_payload.sh
│       ├── dml-discard-empty.service
│       ├── dml-discard-set-ml.service
│       ├── dml-discard.slice
│       ├── dml-override-empty.service
│       ├── dml-override.slice
│       ├── dml-passthrough-empty.service
│       ├── dml-passthrough-set-dml.service
│       ├── dml-passthrough-set-ml.service
│       ├── dml-passthrough.slice
│       ├── dml.slice
│       ├── e.service
│       ├── end.service
│       ├── end.sh
│       ├── f.service
│       ├── g.service
│       ├── generator-utils.sh
│       ├── grandchild.service
│       ├── h.service
│       ├── i.service
│       ├── loopy.service
│       ├── loopy.service.d
│       │   └── compat.conf
│       ├── loopy2.service
│       ├── loopy3.service
│       ├── loopy4.service
│       ├── nomem.slice
│       ├── nomemleaf.service
│       ├── parent-deep.slice
│       ├── parent.slice
│       ├── sched_idle_bad.service
│       ├── sched_idle_ok.service
│       ├── sched_rr_bad.service
│       ├── sched_rr_change.service
│       ├── sched_rr_ok.service
│       ├── shutdown.target
│       ├── sockets.target
│       ├── son.service
│       ├── success-failure-test-failure.service
│       ├── success-failure-test-success.service
│       ├── success-failure-test.service
│       ├── sysinit.target
│       ├── TEST-01-BASIC.sh
│       ├── TEST-02-UNITTESTS.sh
│       ├── TEST-03-JOBS.sh
│       ├── TEST-04-JOURNAL.bsod.sh
│       ├── TEST-04-JOURNAL.cat.sh
│       ├── TEST-04-JOURNAL.corrupted-journals.sh
│       ├── TEST-04-JOURNAL.fss.sh
│       ├── TEST-04-JOURNAL.invocation.sh
│       ├── TEST-04-JOURNAL.journal-append.sh
│       ├── TEST-04-JOURNAL.journal-corrupt.sh
│       ├── TEST-04-JOURNAL.journal-gatewayd.sh
│       ├── TEST-04-JOURNAL.journal-reload.sh
│       ├── TEST-04-JOURNAL.journal-remote.sh
│       ├── TEST-04-JOURNAL.journal.sh
│       ├── TEST-04-JOURNAL.LogFilterPatterns.sh
│       ├── TEST-04-JOURNAL.sh
│       ├── TEST-04-JOURNAL.stopped-socket-activation.sh
│       ├── TEST-04-JOURNAL.SYSTEMD_JOURNAL_COMPRESS.sh
│       ├── TEST-05-RLIMITS.effective-limit.sh
│       ├── TEST-05-RLIMITS.rlimit.sh
│       ├── TEST-05-RLIMITS.sh
│       ├── TEST-06-SELINUX.sh
│       ├── TEST-07-PID1.concurrency.sh
│       ├── TEST-07-PID1.delegate-namespaces.sh
│       ├── TEST-07-PID1.exec-context.sh
│       ├── TEST-07-PID1.exec-deserialization.sh
│       ├── TEST-07-PID1.exec-timestamps.sh
│       ├── TEST-07-PID1.issue-14566.sh
│       ├── TEST-07-PID1.issue-16115.sh
│       ├── TEST-07-PID1.issue-1981.sh
│       ├── TEST-07-PID1.issue-2467.sh
│       ├── TEST-07-PID1.issue-27953.sh
│       ├── TEST-07-PID1.issue-30412.sh
│       ├── TEST-07-PID1.issue-3166.sh
│       ├── TEST-07-PID1.issue-3171.sh
│       ├── TEST-07-PID1.issue-31752.sh
│       ├── TEST-07-PID1.issue-33672.sh
│       ├── TEST-07-PID1.issue-34104.sh
│       ├── TEST-07-PID1.issue-35882.sh
│       ├── TEST-07-PID1.main-PID-change.sh
│       ├── TEST-07-PID1.mount-invalid-chars.sh
│       ├── TEST-07-PID1.mqueue-ownership.sh
│       ├── TEST-07-PID1.poll-limit.sh
│       ├── TEST-07-PID1.pr-31351.sh
│       ├── TEST-07-PID1.prefix-shell.sh
│       ├── TEST-07-PID1.private-bpf.sh
│       ├── TEST-07-PID1.private-network.sh
│       ├── TEST-07-PID1.private-pids.sh
│       ├── TEST-07-PID1.private-users.sh
│       ├── TEST-07-PID1.protect-control-groups.sh
│       ├── TEST-07-PID1.protect-hostname.sh
│       ├── TEST-07-PID1.quota.sh
│       ├── TEST-07-PID1.sh
│       ├── TEST-07-PID1.socket-defer.sh
│       ├── TEST-07-PID1.socket-max-connection.sh
│       ├── TEST-07-PID1.socket-on-failure.sh
│       ├── TEST-07-PID1.socket-pass-fds.sh
│       ├── TEST-07-PID1.startv.sh
│       ├── TEST-07-PID1.subgroup-kill.sh
│       ├── TEST-07-PID1.transient-unit-container.sh
│       ├── TEST-07-PID1.transient.sh
│       ├── TEST-07-PID1.type-exec-parallel.sh
│       ├── TEST-07-PID1.working-directory.sh
│       ├── TEST-08-INITRD.sh
│       ├── TEST-09-REBOOT.journal.sh
│       ├── TEST-09-REBOOT.sh
│       ├── TEST-13-NSPAWN.importctl.sh
│       ├── TEST-13-NSPAWN.machined.sh
│       ├── TEST-13-NSPAWN.nspawn-oci.sh
│       ├── TEST-13-NSPAWN.nspawn.sh
│       ├── TEST-13-NSPAWN.nss-mymachines.sh
│       ├── TEST-13-NSPAWN.sh
│       ├── TEST-13-NSPAWN.unpriv.sh
│       ├── TEST-15-DROPIN.sh
│       ├── TEST-16-EXTEND-TIMEOUT.sh
│       ├── TEST-17-UDEV.buffer-size.sh
│       ├── TEST-17-UDEV.credentials.sh
│       ├── TEST-17-UDEV.database.sh
│       ├── TEST-17-UDEV.device_is_processing.sh
│       ├── TEST-17-UDEV.diskseq.sh
│       ├── TEST-17-UDEV.failed-event.sh
│       ├── TEST-17-UDEV.global-property.sh
│       ├── TEST-17-UDEV.IMPORT.sh
│       ├── TEST-17-UDEV.link-property.sh
│       ├── TEST-17-UDEV.loop-own.sh
│       ├── TEST-17-UDEV.netif-altname.sh
│       ├── TEST-17-UDEV.netif-INTERFACE-property.sh
│       ├── TEST-17-UDEV.owner-and-mode.sh
│       ├── TEST-17-UDEV.queued-events-serialization.sh
│       ├── TEST-17-UDEV.rename-netif.sh
│       ├── TEST-17-UDEV.sanity-check.sh
│       ├── TEST-17-UDEV.sh
│       ├── TEST-17-UDEV.SYSTEMD_ALIAS.sh
│       ├── TEST-17-UDEV.SYSTEMD_WANTS_vs_StopWhenUnneeded.sh
│       ├── TEST-17-UDEV.SYSTEMD_WANTS-escape.sh
│       ├── TEST-17-UDEV.SYSTEMD_WANTS.sh
│       ├── TEST-17-UDEV.TAG.sh
│       ├── TEST-17-UDEV.verify.sh
│       ├── TEST-17-UDEV.watch.sh
│       ├── TEST-18-FAILUREACTION.sh
│       ├── TEST-19-CGROUP.cleanup-slice.sh
│       ├── TEST-19-CGROUP.delegate.sh
│       ├── TEST-19-CGROUP.ExitType-cgroup.sh
│       ├── TEST-19-CGROUP.IPAddressAllow-Deny.sh
│       ├── TEST-19-CGROUP.keyed-properties.sh
│       ├── TEST-19-CGROUP.sh
│       ├── TEST-21-DFUZZER.sh
│       ├── TEST-22-TMPFILES.01.sh
│       ├── TEST-22-TMPFILES.02.sh
│       ├── TEST-22-TMPFILES.03.sh
│       ├── TEST-22-TMPFILES.04.sh
│       ├── TEST-22-TMPFILES.05.sh
│       ├── TEST-22-TMPFILES.06.sh
│       ├── TEST-22-TMPFILES.07.sh
│       ├── TEST-22-TMPFILES.08.sh
│       ├── TEST-22-TMPFILES.09.sh
│       ├── TEST-22-TMPFILES.10.sh
│       ├── TEST-22-TMPFILES.11.sh
│       ├── TEST-22-TMPFILES.12.sh
│       ├── TEST-22-TMPFILES.13.sh
│       ├── TEST-22-TMPFILES.14.sh
│       ├── TEST-22-TMPFILES.15.sh
│       ├── TEST-22-TMPFILES.16.sh
│       ├── TEST-22-TMPFILES.17.sh
│       ├── TEST-22-TMPFILES.18.sh
│       ├── TEST-22-TMPFILES.19.sh
│       ├── TEST-22-TMPFILES.20.sh
│       ├── TEST-22-TMPFILES.21.sh
│       ├── TEST-22-TMPFILES.sh
│       ├── TEST-23-UNIT-FILE-ExtraFileDescriptors-child.sh
│       ├── TEST-23-UNIT-FILE-openfile-child.sh
│       ├── TEST-23-UNIT-FILE-short-lived.sh
│       ├── TEST-23-UNIT-FILE.clean-unit.sh
│       ├── TEST-23-UNIT-FILE.exec-command-ex.sh
│       ├── TEST-23-UNIT-FILE.ExecReload.sh
│       ├── TEST-23-UNIT-FILE.ExecStopPost.sh
│       ├── TEST-23-UNIT-FILE.ExtraFileDescriptors.sh
│       ├── TEST-23-UNIT-FILE.JoinsNamespaceOf.sh
│       ├── TEST-23-UNIT-FILE.oneshot-restart.sh
│       ├── TEST-23-UNIT-FILE.openfile.sh
│       ├── TEST-23-UNIT-FILE.percentj-wantedby.sh
│       ├── TEST-23-UNIT-FILE.runtime-bind-paths.sh
│       ├── TEST-23-UNIT-FILE.RuntimeDirectory.sh
│       ├── TEST-23-UNIT-FILE.sh
│       ├── TEST-23-UNIT-FILE.StandardOutput.sh
│       ├── TEST-23-UNIT-FILE.start-stop-no-reload.sh
│       ├── TEST-23-UNIT-FILE.statedir.sh
│       ├── TEST-23-UNIT-FILE.success-failure.sh
│       ├── TEST-23-UNIT-FILE.type-exec.sh
│       ├── TEST-23-UNIT-FILE.Upholds.sh
│       ├── TEST-23-UNIT-FILE.utmp.sh
│       ├── TEST-23-UNIT-FILE.verify-unit-files.sh
│       ├── TEST-23-UNIT-FILE.whoami.sh
│       ├── TEST-24-CRYPTSETUP.sh
│       ├── TEST-25-IMPORT.sh
│       ├── TEST-26-SYSTEMCTL.sh
│       ├── TEST-29-PORTABLE.directory.sh
│       ├── TEST-29-PORTABLE.image.sh
│       ├── TEST-29-PORTABLE.sh
│       ├── TEST-30-ONCLOCKCHANGE.sh
│       ├── TEST-31-DEVICE-ENUMERATION.sh
│       ├── TEST-32-OOMPOLICY.sh
│       ├── TEST-34-DYNAMICUSERMIGRATE.sh
│       ├── TEST-35-LOGIN.sh
│       ├── TEST-36-NUMAPOLICY.sh
│       ├── TEST-38-FREEZER-sleep.service
│       ├── TEST-38-FREEZER.sh
│       ├── TEST-43-PRIVATEUSER-UNPRIV.sh
│       ├── TEST-44-LOG-NAMESPACE.sh
│       ├── TEST-45-TIMEDATE.sh
│       ├── TEST-46-HOMED.sh
│       ├── TEST-50-DISSECT.DDI.sh
│       ├── TEST-50-DISSECT.dissect.sh
│       ├── TEST-50-DISSECT.mountfsd.sh
│       ├── TEST-50-DISSECT.sh
│       ├── TEST-50-DISSECT.sysext.sh
│       ├── TEST-52-HONORFIRSTSHUTDOWN.sh
│       ├── TEST-53-ISSUE-16347.sh
│       ├── TEST-54-CREDS.sh
│       ├── TEST-55-OOMD-testbloat.service
│       ├── TEST-55-OOMD-testchill.service
│       ├── TEST-55-OOMD-testmunch.service
│       ├── TEST-55-OOMD-workload.slice
│       ├── TEST-55-OOMD-workload.slice.d
│       │   └── 99-oom.conf
│       ├── TEST-55-OOMD.sh
│       ├── TEST-58-REPART.sh
│       ├── TEST-59-RELOADING-RESTART.sh
│       ├── TEST-60-MOUNT-RATELIMIT.sh
│       ├── TEST-62-RESTRICT-IFACES-1.service
│       ├── TEST-62-RESTRICT-IFACES-2.service
│       ├── TEST-62-RESTRICT-IFACES-3.service
│       ├── TEST-62-RESTRICT-IFACES-4.service
│       ├── TEST-62-RESTRICT-IFACES-5.service
│       ├── TEST-62-RESTRICT-IFACES-6.service
│       ├── TEST-62-RESTRICT-IFACES.sh
│       ├── TEST-63-PATH.sh
│       ├── TEST-64-UDEV-STORAGE.sh
│       ├── TEST-65-ANALYZE.sh
│       ├── TEST-66-DEVICE-ISOLATION-device-isolation.service
│       ├── TEST-66-DEVICE-ISOLATION.sh
│       ├── TEST-67-INTEGRITY.sh
│       ├── TEST-68-PROPAGATE-EXIT-STATUS.sh
│       ├── TEST-69-SHUTDOWN.py
│       ├── TEST-70-TPM2.creds.sh
│       ├── TEST-70-TPM2.cryptenroll.sh
│       ├── TEST-70-TPM2.cryptsetup.sh
│       ├── TEST-70-TPM2.measure.sh
│       ├── TEST-70-TPM2.pcrextend.sh
│       ├── TEST-70-TPM2.pcrlock.sh
│       ├── TEST-70-TPM2.sh
│       ├── TEST-70-TPM2.tpm2-setup.sh
│       ├── TEST-71-HOSTNAME.sh
│       ├── TEST-72-SYSUPDATE.sh
│       ├── TEST-73-LOCALE.sh
│       ├── TEST-74-AUX-UTILS.ask-password.sh
│       ├── TEST-74-AUX-UTILS.battery-check.sh
│       ├── TEST-74-AUX-UTILS.busctl.sh
│       ├── TEST-74-AUX-UTILS.capsule.sh
│       ├── TEST-74-AUX-UTILS.cgls.sh
│       ├── TEST-74-AUX-UTILS.cgtop.sh
│       ├── TEST-74-AUX-UTILS.defer_reactivation.sh
│       ├── TEST-74-AUX-UTILS.delta.sh
│       ├── TEST-74-AUX-UTILS.detect-virt.sh
│       ├── TEST-74-AUX-UTILS.escape.sh
│       ├── TEST-74-AUX-UTILS.firstboot.sh
│       ├── TEST-74-AUX-UTILS.id128.sh
│       ├── TEST-74-AUX-UTILS.keyutil.sh
│       ├── TEST-74-AUX-UTILS.machine-id-setup.sh
│       ├── TEST-74-AUX-UTILS.mount.sh
│       ├── TEST-74-AUX-UTILS.network-generator.sh
│       ├── TEST-74-AUX-UTILS.networkctl.sh
│       ├── TEST-74-AUX-UTILS.path.sh
│       ├── TEST-74-AUX-UTILS.pty-forward.sh
│       ├── TEST-74-AUX-UTILS.run.sh
│       ├── TEST-74-AUX-UTILS.sbsign.sh
│       ├── TEST-74-AUX-UTILS.sh
│       ├── TEST-74-AUX-UTILS.socket-activate.sh
│       ├── TEST-74-AUX-UTILS.ssh.sh
│       ├── TEST-74-AUX-UTILS.sysusers.sh
│       ├── TEST-74-AUX-UTILS.userdbctl.sh
│       ├── TEST-74-AUX-UTILS.varlinkctl.sh
│       ├── TEST-74-AUX-UTILS.vpick.sh
│       ├── TEST-75-RESOLVED.sh
│       ├── TEST-76-SYSCTL.sh
│       ├── TEST-78-SIGQUEUE.sh
│       ├── TEST-79-MEMPRESS.sh
│       ├── TEST-80-NOTIFYACCESS.sh
│       ├── TEST-81-GENERATORS.debug-generator.sh
│       ├── TEST-81-GENERATORS.environment-d-generator.sh
│       ├── TEST-81-GENERATORS.fstab-generator.sh
│       ├── TEST-81-GENERATORS.getty-generator.sh
│       ├── TEST-81-GENERATORS.run-generator.sh
│       ├── TEST-81-GENERATORS.sh
│       ├── TEST-81-GENERATORS.system-update-generator.sh
│       ├── TEST-82-SOFTREBOOT.sh
│       ├── TEST-83-BTRFS.sh
│       ├── TEST-84-STORAGETM.sh
│       ├── TEST-86-MULTI-PROFILE-UKI.sh
│       ├── TEST-87-AUX-UTILS-VM.bootctl.sh
│       ├── TEST-87-AUX-UTILS-VM.coredump.sh
│       ├── TEST-87-AUX-UTILS-VM.detect-virt.sh
│       ├── TEST-87-AUX-UTILS-VM.modules-load.sh
│       ├── TEST-87-AUX-UTILS-VM.mount.sh
│       ├── TEST-87-AUX-UTILS-VM.pstore.sh
│       ├── TEST-87-AUX-UTILS-VM.sh
│       ├── TEST-87-AUX-UTILS-VM.validatefs.sh
│       ├── TEST-88-UPGRADE.sh
│       ├── test-control.sh
│       ├── testsuite.target
│       ├── timers.target
│       ├── unit-.service.d
│       │   └── 10-override.conf
│       ├── unit-with-.service.d
│       │   └── 20-override.conf
│       ├── unit-with-multiple-.service.d
│       │   ├── 20-override.conf
│       │   └── 30-override.conf
│       ├── unit-with-multiple-dashes.service
│       ├── unit-with-multiple-dashes.service.d
│       │   └── 10-override.conf
│       └── util.sh
├── tmpfiles.d
│   ├── 20-systemd-osc-context.conf.in
│   ├── 20-systemd-shell-extra.conf.in
│   ├── 20-systemd-ssh-generator.conf.in
│   ├── 20-systemd-stub.conf.in
│   ├── 20-systemd-userdb.conf.in
│   ├── credstore.conf
│   ├── etc.conf.in
│   ├── home.conf
│   ├── journal-nocow.conf
│   ├── legacy.conf.in
│   ├── meson.build
│   ├── portables.conf
│   ├── provision.conf
│   ├── README
│   ├── static-nodes-permissions.conf.in
│   ├── systemd-network.conf
│   ├── systemd-nologin.conf
│   ├── systemd-nspawn.conf
│   ├── systemd-pstore.conf
│   ├── systemd-resolve.conf
│   ├── systemd-tmp.conf
│   ├── systemd.conf.in
│   ├── tmp.conf
│   ├── var.conf.in
│   └── x11.conf
├── TODO
├── tools
│   ├── analyze-dump-sort.py
│   ├── catalog-report.py
│   ├── check-api-docs.sh
│   ├── check-efi-alignment.py
│   ├── check-help.sh
│   ├── check-version-history.py
│   ├── check-version.sh
│   ├── chromiumos
│   │   └── gen_autosuspend_rules.py
│   ├── command_ignorelist
│   ├── coverity.sh
│   ├── dbus_exporter.py
│   ├── dbus_ignorelist
│   ├── debug-sd-boot.sh
│   ├── dump-auxv.py
│   ├── elf2efi.py
│   ├── fetch-distro.py
│   ├── fetch-mkosi.py
│   ├── find-build-dir.sh
│   ├── find-double-newline.sh
│   ├── find-tabs.sh
│   ├── function_ignorelist
│   ├── gdb-sd_dump_hashmaps.py
│   ├── generate-gperfs.py
│   ├── git-contrib.sh
│   ├── git-setup.sh
│   ├── list-discoverable-partitions.py
│   ├── make-autosuspend-rules.py
│   ├── make-directive-index.py
│   ├── make-man-index.py
│   ├── meson-build.sh
│   ├── meson-extract-unit-files.py
│   ├── meson-render-jinja2.py
│   ├── oss-fuzz.sh
│   ├── sync-docs.py
│   ├── update-dbus-docs.py
│   ├── update-hwdb-autosuspend.sh
│   ├── update-hwdb.sh
│   ├── update-man-rules.py
│   ├── update-syscall-tables.sh
│   ├── vcs-tag.sh
│   └── xml_helper.py
├── units
│   ├── basic.target
│   ├── blockdev@.target
│   ├── bluetooth.target
│   ├── boot-complete.target
│   ├── breakpoint-pre-basic.service.in
│   ├── breakpoint-pre-mount.service.in
│   ├── breakpoint-pre-switch-root.service.in
│   ├── breakpoint-pre-udev.service.in
│   ├── capsule.slice
│   ├── capsule@.service.in
│   ├── console-getty.service.in
│   ├── container-getty@.service.in
│   ├── cryptsetup-pre.target
│   ├── cryptsetup.target
│   ├── debug-shell.service.in
│   ├── dev-hugepages.mount
│   ├── dev-mqueue.mount
│   ├── emergency.service.in
│   ├── emergency.target
│   ├── exit.target
│   ├── factory-reset-now.target
│   ├── factory-reset.target
│   ├── final.target
│   ├── first-boot-complete.target
│   ├── getty-pre.target
│   ├── getty.target
│   ├── getty@.service.in
│   ├── graphical.target
│   ├── halt.target
│   ├── hibernate.target
│   ├── hybrid-sleep.target
│   ├── imports-pre.target
│   ├── imports.target
│   ├── initrd-cleanup.service
│   ├── initrd-fs.target
│   ├── initrd-parse-etc.service.in
│   ├── initrd-root-device.target
│   ├── initrd-root-fs.target
│   ├── initrd-switch-root.service
│   ├── initrd-switch-root.target
│   ├── initrd-udevadm-cleanup-db.service
│   ├── initrd-usr-fs.target
│   ├── initrd.target
│   ├── integritysetup-pre.target
│   ├── integritysetup.target
│   ├── kexec.target
│   ├── kmod-static-nodes.service.in
│   ├── ldconfig.service
│   ├── local-fs-pre.target
│   ├── local-fs.target
│   ├── machine.slice
│   ├── machines.target
│   ├── meson.build
│   ├── modprobe@.service
│   ├── multi-user.target
│   ├── network-online.target
│   ├── network-pre.target
│   ├── network.target
│   ├── nss-lookup.target
│   ├── nss-user-lookup.target
│   ├── paths.target
│   ├── poweroff.target
│   ├── printer.target
│   ├── proc-sys-fs-binfmt_misc.automount
│   ├── proc-sys-fs-binfmt_misc.mount
│   ├── quotaon-root.service.in
│   ├── quotaon@.service.in
│   ├── rc-local.service.in
│   ├── reboot.target
│   ├── remote-cryptsetup.target
│   ├── remote-fs-pre.target
│   ├── remote-fs.target
│   ├── remote-integritysetup.target
│   ├── remote-veritysetup.target
│   ├── rescue.service.in
│   ├── rescue.target
│   ├── rpcbind.target
│   ├── serial-getty@.service.in
│   ├── shutdown.target
│   ├── sigpwr.target
│   ├── sleep.target
│   ├── slices.target
│   ├── smartcard.target
│   ├── sockets.target
│   ├── soft-reboot.target
│   ├── sound.target
│   ├── ssh-access.target
│   ├── storage-target-mode.target
│   ├── suspend-then-hibernate.target
│   ├── suspend.target
│   ├── swap.target
│   ├── sys-fs-fuse-connections.mount
│   ├── sys-kernel-config.mount
│   ├── sys-kernel-debug.mount
│   ├── sys-kernel-tracing.mount
│   ├── sysinit.target
│   ├── syslog.socket
│   ├── system-systemd\x2dcryptsetup.slice
│   ├── system-systemd\x2dveritysetup.slice
│   ├── system-update-cleanup.service
│   ├── system-update-pre.target
│   ├── system-update.target
│   ├── systemd-ask-password-console.path
│   ├── systemd-ask-password-console.service
│   ├── systemd-ask-password-wall.path
│   ├── systemd-ask-password-wall.service
│   ├── systemd-ask-password.socket
│   ├── systemd-ask-password@.service
│   ├── systemd-backlight@.service.in
│   ├── systemd-battery-check.service.in
│   ├── systemd-binfmt.service.in
│   ├── systemd-bless-boot.service.in
│   ├── systemd-boot-check-no-failures.service.in
│   ├── systemd-boot-clear-sysfail.service
│   ├── systemd-boot-random-seed.service
│   ├── systemd-boot-update.service
│   ├── systemd-bootctl.socket
│   ├── systemd-bootctl@.service
│   ├── systemd-bsod.service.in
│   ├── systemd-confext-initrd.service
│   ├── systemd-confext.service
│   ├── systemd-coredump.socket
│   ├── systemd-coredump@.service.in
│   ├── systemd-creds.socket
│   ├── systemd-creds@.service
│   ├── systemd-exit.service
│   ├── systemd-factory-reset-complete.service.in
│   ├── systemd-factory-reset-reboot.service
│   ├── systemd-factory-reset-request.service.in
│   ├── systemd-factory-reset.socket
│   ├── systemd-factory-reset@.service.in
│   ├── systemd-firstboot.service
│   ├── systemd-fsck-root.service.in
│   ├── systemd-fsck@.service.in
│   ├── systemd-growfs-root.service.in
│   ├── systemd-growfs@.service.in
│   ├── systemd-halt.service
│   ├── systemd-hibernate-clear.service.in
│   ├── systemd-hibernate-resume.service.in
│   ├── systemd-hibernate.service.in
│   ├── systemd-homed-activate.service
│   ├── systemd-homed-firstboot.service
│   ├── systemd-homed.service.in
│   ├── systemd-hostnamed.service.in
│   ├── systemd-hostnamed.socket
│   ├── systemd-hwdb-update.service.in
│   ├── systemd-hybrid-sleep.service.in
│   ├── systemd-importd.service.in
│   ├── systemd-importd.socket
│   ├── systemd-journal-catalog-update.service
│   ├── systemd-journal-flush.service
│   ├── systemd-journal-gatewayd.service.in
│   ├── systemd-journal-gatewayd.socket
│   ├── systemd-journal-remote.service.in
│   ├── systemd-journal-remote.socket
│   ├── systemd-journal-upload.service.in
│   ├── systemd-journald-audit.socket
│   ├── systemd-journald-dev-log.socket
│   ├── systemd-journald-sync@.service
│   ├── systemd-journald-varlink@.socket
│   ├── systemd-journald.service.in
│   ├── systemd-journald.socket
│   ├── systemd-journald@.service.in
│   ├── systemd-journald@.socket
│   ├── systemd-kexec.service
│   ├── systemd-localed.service.in
│   ├── systemd-logind-varlink.socket
│   ├── systemd-logind.service.in
│   ├── systemd-loop@.service
│   ├── systemd-machine-id-commit.service
│   ├── systemd-machined.service.in
│   ├── systemd-machined.socket
│   ├── systemd-modules-load.service.in
│   ├── systemd-mountfsd.service.in
│   ├── systemd-mountfsd.socket
│   ├── systemd-network-generator.service.in
│   ├── systemd-networkd-persistent-storage.service
│   ├── systemd-networkd-varlink.socket
│   ├── systemd-networkd-wait-online.service.in
│   ├── systemd-networkd-wait-online@.service.in
│   ├── systemd-networkd.service.in
│   ├── systemd-networkd.socket
│   ├── systemd-nspawn@.service.in
│   ├── systemd-nsresourced.service.in
│   ├── systemd-nsresourced.socket
│   ├── systemd-oomd.service.in
│   ├── systemd-oomd.socket
│   ├── systemd-pcrextend.socket
│   ├── systemd-pcrextend@.service.in
│   ├── systemd-pcrfs-root.service.in
│   ├── systemd-pcrfs@.service.in
│   ├── systemd-pcrlock-file-system.service.in
│   ├── systemd-pcrlock-firmware-code.service.in
│   ├── systemd-pcrlock-firmware-config.service.in
│   ├── systemd-pcrlock-machine-id.service.in
│   ├── systemd-pcrlock-make-policy.service.in
│   ├── systemd-pcrlock-secureboot-authority.service.in
│   ├── systemd-pcrlock-secureboot-policy.service.in
│   ├── systemd-pcrlock.socket
│   ├── systemd-pcrlock@.service.in
│   ├── systemd-pcrmachine.service.in
│   ├── systemd-pcrphase-factory-reset.service.in
│   ├── systemd-pcrphase-initrd.service.in
│   ├── systemd-pcrphase-storage-target-mode.service.in
│   ├── systemd-pcrphase-sysinit.service.in
│   ├── systemd-pcrphase.service.in
│   ├── systemd-portabled.service.in
│   ├── systemd-poweroff.service
│   ├── systemd-pstore.service.in
│   ├── systemd-quotacheck-root.service.in
│   ├── systemd-quotacheck@.service.in
│   ├── systemd-random-seed.service.in
│   ├── systemd-reboot.service
│   ├── systemd-remount-fs.service.in
│   ├── systemd-repart.service
│   ├── systemd-resolved-monitor.socket
│   ├── systemd-resolved-varlink.socket
│   ├── systemd-resolved.service.in
│   ├── systemd-rfkill.service.in
│   ├── systemd-rfkill.socket
│   ├── systemd-soft-reboot.service
│   ├── systemd-storagetm.service.in
│   ├── systemd-suspend-then-hibernate.service.in
│   ├── systemd-suspend.service.in
│   ├── systemd-sysctl.service.in
│   ├── systemd-sysext-initrd.service
│   ├── systemd-sysext.service
│   ├── systemd-sysext.socket
│   ├── systemd-sysext@.service
│   ├── systemd-sysupdate-reboot.service.in
│   ├── systemd-sysupdate-reboot.timer
│   ├── systemd-sysupdate.service.in
│   ├── systemd-sysupdate.timer
│   ├── systemd-sysupdated.service.in
│   ├── systemd-sysusers.service
│   ├── systemd-time-wait-sync.service.in
│   ├── systemd-timedated.service.in
│   ├── systemd-timesyncd.service.in
│   ├── systemd-tmpfiles-clean.service
│   ├── systemd-tmpfiles-clean.timer
│   ├── systemd-tmpfiles-setup-dev-early.service
│   ├── systemd-tmpfiles-setup-dev.service
│   ├── systemd-tmpfiles-setup.service
│   ├── systemd-tpm2-clear.service.in
│   ├── systemd-tpm2-setup-early.service.in
│   ├── systemd-tpm2-setup.service.in
│   ├── systemd-udev-load-credentials.service
│   ├── systemd-udev-settle.service
│   ├── systemd-udev-trigger.service
│   ├── systemd-udevd-control.socket
│   ├── systemd-udevd-kernel.socket
│   ├── systemd-udevd-varlink.socket
│   ├── systemd-udevd.service.in
│   ├── systemd-update-done.service.in
│   ├── systemd-update-utmp.service.in
│   ├── systemd-user-sessions.service.in
│   ├── systemd-userdb-load-credentials.service
│   ├── systemd-userdbd.service.in
│   ├── systemd-userdbd.socket
│   ├── systemd-validatefs@.service.in
│   ├── systemd-vconsole-setup.service.in
│   ├── systemd-vmspawn@.service.in
│   ├── systemd-volatile-root.service.in
│   ├── time-set.target
│   ├── time-sync.target
│   ├── timers.target
│   ├── tmp.mount
│   ├── tpm2.target
│   ├── umount.target
│   ├── usb-gadget.target
│   ├── user
│   │   ├── app.slice
│   │   ├── background.slice
│   │   ├── basic.target
│   │   ├── bluetooth.target
│   │   ├── capsule@.target
│   │   ├── default.target
│   │   ├── exit.target
│   │   ├── graphical-session-pre.target
│   │   ├── graphical-session.target
│   │   ├── machine.slice
│   │   ├── machines.target
│   │   ├── meson.build
│   │   ├── paths.target
│   │   ├── printer.target
│   │   ├── session.slice
│   │   ├── shutdown.target
│   │   ├── smartcard.target
│   │   ├── sockets.target
│   │   ├── sound.target
│   │   ├── systemd-ask-password.socket
│   │   ├── systemd-ask-password@.service
│   │   ├── systemd-exit.service
│   │   ├── systemd-nspawn@.service.in
│   │   ├── systemd-tmpfiles-clean.service
│   │   ├── systemd-tmpfiles-clean.timer
│   │   ├── systemd-tmpfiles-setup.service
│   │   ├── systemd-vmspawn@.service.in
│   │   ├── timers.target
│   │   └── xdg-desktop-autostart.target
│   ├── user-.slice.d
│   │   └── 10-defaults.conf
│   ├── user-runtime-dir@.service.in
│   ├── user.slice
│   ├── user@.service.d
│   │   └── 10-login-barrier.conf
│   ├── user@.service.in
│   ├── user@0.service.d
│   │   └── 10-login-barrier.conf
│   ├── var-lib-machines.mount
│   ├── veritysetup-pre.target
│   └── veritysetup.target
└── xorg
    └── 50-systemd-user.sh

591 directories, 6557 files
