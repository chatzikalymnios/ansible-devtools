# K3D Ansible Role

This role can be used to install [K3D](https://k3d.io/) on a Linux development workstation.

## Example Playbook

```yml
# ansible-playbook -K -i localhost, playbook.yml
- hosts: all
  connection: local
  gather_facts: yes
  roles:
    - role: k3d
```
