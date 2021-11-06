# Docker Engine Ansible Role

This role can be used to install the Docker Engine on an Ubuntu development workstation.

## Role Variables

The role uses variables defined in `defaults/main.yml`.

### `arch`

- System architecture
- Default value: derived from `{{ ansible_architecture }}`

### `lsb_release`

- The Ubuntu release codename
- Default value: `{{ ansible_lsb.codename }}`

## Example Playbook

```yml
# ansible-playbook -K -i localhost, playbook.yml
- hosts: all
  connection: local
  gather_facts: yes
  roles:
    - role: docker
      arch: amd64
      lsb_release: focal
```
