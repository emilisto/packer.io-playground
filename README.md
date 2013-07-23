# Playing with packer.io

Go check out [packer.io](http://packer.io/)!

To build your own Ubuntu 13.04 Vagrant box:

1. [Install Packer](http://www.packer.io/intro/getting-started/setup.html)
2. Run `cd output && packer build template.json`
`

## Building the VMware Fusion box

It failed when running `vbox.sh` - obviously. Apparently the guest
additions for Fusion are part of the open [open-vm-tools](http://open-vm-tools.sourceforge.net/).

## Random notes of mine

- gem install veewee-to-packer
- Cloned veewee and copied `templates/ubuntu-13.04-server-adm64` out of
the repository
- Ran weevee-to-packer on `templates/ubuntu-13.04-server-adm64/definitions.rb`
- Idea: create an ISO from an already generated box and use it as the
start AMI for another box. Might speed up the process. Although — it
might be pointless since it imposes complexity, and the time it takes to
build from scratch isn't so long after all.
