In Debian/Ubuntu, if `/etc/interfaces` file is changed, `service networking restart` won't help. It expects ip addresses from new file to exist on interfaces. Addresses from old file will be left. This is realy annoying, if you are editing interfaces file with SCM like Ansible/Puppet/whatever. This script restarts all interfaces, except loopback.

**P.S.** If this code is useful for you - don't forget to put a star on it's [github repo](https://github.com/selivan/ansible-debian-networking-correct-restart).
