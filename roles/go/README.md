# Go Ansible Role

This role can be used to install or upgrade/downgrade [Go](https://golang.org/) on a Linux development workstation.

## Role Variables and Defaults

```yml
# the version of Go to install
version: latest

# the system architecture
arch: derived from {{ ansible_architecture }}

# the directory in which to extract the archive
prefix: /usr/local

# the directory in which to create symlinks for the Go binaries
bindir: /usr/local/bin
```

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
