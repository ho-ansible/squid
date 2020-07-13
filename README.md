# Ansible role: squid
HTTP/S proxy

## Requirements
Only tested on Debian stable, for now.

## Role Variables

## Dependencies
+ [ho-ansible.systemd](https://github.com/ho-ansible/systemd)

## Example Playbook

```
- hosts: all
  roles:
    - { role: ho-ansible.squid }
```

## License
MIT

## Author Information
Sean Ho, https://github.com/ho-ansible/
