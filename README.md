# Playing with packer.io

Go check out [packer.io](http://packer.io/)!

To build your own Ubuntu 13.04 Vagrant box:

1. [Install Packer](http://www.packer.io/intro/getting-started/setup.html)
2. Run `cd output && packer build template.json`
`

## Random notes of mine

- gem install veewee-to-packer
- Cloned veewee and copied `templates/ubuntu-13.04-server-adm64` out of
the repository
- Ran weevee-to-packer on `templates/ubuntu-13.04-server-adm64/definitions.rb`
