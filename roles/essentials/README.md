# Essentials Ansible Role

This role can be used to install essential packages for development on an Ubuntu system.

## Packages

The following packages will be installed.

- `build-essential`
- `curl`
- `git`
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
