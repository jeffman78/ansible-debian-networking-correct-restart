ansible-debian-networking-restart
=================================

In Debian/Ubuntu, if interfaces file changed, `service networking restart` won't help. It expects ip addresses from new file to exist on interfaces. Addresses from old file will be left. This is realy annoying, if you are editing interfaces file with SCM like Ansible/Puppet/whatever. This script restarts all interfaces, except lo.

