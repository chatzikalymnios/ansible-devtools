# Development Tools Collection for Ansible

This is a collection of ansible roles I use to set up development tools on my workstation. I use Ubuntu, so YMMV with other distributions.

## Roles

- [go](roles/go)

## Using this collection

Make sure `ansible` is installed.

```sh
pip3 install --upgrade --upgrade-strategy=eager ansible
```

Edit `playbook.yml` to include the needed roles and run the following command.

```sh
ansible-playbook -K -i localhost, playbook.yml
```
