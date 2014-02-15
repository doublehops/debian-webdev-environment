Easy webdev environment installation
==============

Build your next webdev environment easily by running a single script. You will need to have recent versions of both Vagrant and Ansible installed.

## What will be installed
- Debian 7
- PHP 5 (latest version)
- Nginx (latest version)
- MariaDB

## Installing and configuring the vm
Once Vagrant, Ansible and virtualisation software (such as Virtualbox) installed. Check out this repo `git clone git@github.com:doublehops/debian-webdev-environment` into a blank directory and then run `vagrant up`. Run `vagrant provision` to push any Ansible Playbook changes back to the vm. Run `vagrant ssh` to ssh into the vm.

Add a record to /etc/hosts `echo '192.168.33.10 development' | sudo tee -a /etc/hosts` and point your web browser to `http://development/`
