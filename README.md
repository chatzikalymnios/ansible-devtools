# Development Tools Collection for Ansible

This is a collection of ansible roles I use to set up development tools on my Ubuntu system. Some roles explicitly only work on Ubuntu. Others are potentially more broadly applicable, but have not been tested on any other distribution.

## Roles

- [essentials](roles/essentials)
- [go](roles/go)
- [nvm](roles/nvm)
- [sdkman](roles/sdkman)

## Using this collection

Make sure `ansible` is installed.

```sh
sudo apt update && sudo apt install python3-pip
pip3 install --user --upgrade --upgrade-strategy=eager ansible
```

Edit `playbook.yml` to include the needed roles and run the following command.

```sh
ansible-playbook -K -i localhost, playbook.yml
```
