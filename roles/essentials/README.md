# Essentials Ansible Role

This role can be used to install essential packages for development on an Ubuntu system.

## Packages

This role installs the following packages.

- `build-essential`
- `curl`
- `git`
- `htop`
- `vim`

## Example Playbook

```yml
# ansible-playbook -K -i localhost, playbook.yml
- hosts: all
  connection: local
  gather_facts: yes
  roles:
    - role: essentials
```
