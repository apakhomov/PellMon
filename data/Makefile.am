# Dbus policy file
policydir = $(sysconfdir)/dbus-1/system.d
policy_DATA = pellmon_dbus.conf

EXTRA_DIST = \
	pellmon_dbus.conf.in

CLEANFILES = \
	pellmon_dbus.conf

pellmon_dbus.conf: pellmon_dbus.conf.in Makefile
	sed \
		-e 's,[@]user_srv[@],$(user_srv),g' \
		$< > $@

