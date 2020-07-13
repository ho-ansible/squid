# Ansible role: socks-proxy
SOCKS proxy using ssh to localhost.

## Requirements
Only tested on Debian stable, for now.

## Role Variables
+ `socks_listen_ip` (default: 127.0.0.1): IPv4 address on host from which proxy can be accessed.
  Do not set this to 0.0.0.0/0 unless you have VPC firewall rules or similar preventing your
  proxy from being public to the Internet.
+ `socks_listen_port` (default: 1080): TCP port on which proxy can be accessed.
+ `socks_iptables` (default: none): list of iptables rules, e.g., `['-i vpn0 -j ACCEPT']`

## Dependencies
+ [ho-ansible.systemd](https://github.com/ho-ansible/systemd)

## Example Playbook

```
- hosts: all
  roles:
    - { role: ho-ansible.socks-proxy }
```

## License
MIT

## Author Information
Sean Ho, https://github.com/ho-ansible/
