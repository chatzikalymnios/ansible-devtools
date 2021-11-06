# Go Ansible Role

This role can be used to install [nvm](https://github.com/nvm-sh/nvm) on a Linux development workstation.

## Dependencies

This role depends on the [essentials](../essentials) role because it makes use of `curl`.

## Example Playbook

```yml
# ansible-playbook -K -i localhost, playbook.yml
- hosts: all
  connection: local
  gather_facts: yes
  roles:
    - role: nvm
```
