# Go Ansible Role

This role can be used to install or upgrade/downgrade [Go](https://golang.org/) on a Linux development workstation.

## Role Variables

The role uses variables defined in `defaults/main.yml`.

### `version`

- Version to install
- Default value: `latest`

### `arch`

- System architecture
- Default value: derived from `{{ ansible_architecture }}`

### `prefix`

- Directory in which to extract the archive
- Default value: `/usr/local`

### `bindir`

- Directory in which to create symlinks for the binaries
- Default value: `/usr/local/bin`

## Example Playbook

```yml
# ansible-playbook -K -i localhost, playbook.yml
- hosts: all
  connection: local
  gather_facts: yes
  roles:
    - role: go
      version: 1.17.3
      arch: amd64
      prefix: /usr/local
      bindir: /usr/local/bin
```
