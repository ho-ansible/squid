# Ansible role: squid
HTTP/S proxy

## Requirements
Only tested on Debian stable, for now.

## Role Variables
+ `squid_ip` (default: 127.0.0.1): interface to listen on
+ `squid_port` (default: 3128): TCP port to listen on
+ `squid_iptables`: list of additional iptables rules

## Playbooks
+ `main.yml`: apply role
+ `uninstall.yml`: remove. Run before removing config from inventory.

## Dependencies
+ [ho-ansible.systemd](https://github.com/ho-ansible/systemd)

## License
+ Ansible role licensed [MIT](LICENSE)

## Author Information
+ Ansible role by [Sean Ho](https://github.com/ho-ansible/)
