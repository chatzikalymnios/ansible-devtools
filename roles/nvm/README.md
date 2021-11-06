# NVM Ansible Role

This role can be used to install [nvm](https://github.com/nvm-sh/nvm) on an Ubuntu development workstation.

## Example Playbook

```yml
# ansible-playbook -K -i localhost, playbook.yml
- hosts: all
  connection: local
  gather_facts: yes
  roles:
    - role: nvm
```
