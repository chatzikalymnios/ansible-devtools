# QEMU-KVM Ansible Role

This role can be used to install necessary packages for QEMU-KVM virtualization on an Ubuntu system.

## Packages

This role installs the following packages.

- `qemu`
- `qemu-kvm`
- `libvirt-daemon`
- `libvirt-clients`
- `libvirt-dev`
- `bridge-utils`
- `virt-manager`

## Example Playbook

```yml
# ansible-playbook -K -i localhost, playbook.yml
- hosts: all
  connection: local
  gather_facts: yes
  roles:
    - role: qemu-kvm
```
