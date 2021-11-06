# k9s Ansible Role

This role can be used to install the latest version of [k9s](https://k9scli.io/) on a Linux development workstation.

## Role Variables

The role uses variables defined in `defaults/main.yml`.

### `arch`

- System architecture
- Default value: derived from `{{ ansible_architecture }}`

### `bindir`

- Directory in which to extract the binary
- Default value: `/usr/local/bin`

## Example Playbook

```yml
# ansible-playbook -K -i localhost, playbook.yml
- hosts: all
  connection: local
  gather_facts: yes
  roles:
    - role: k9s
      arch: x86_64
      bindir: /usr/local/bin
```
