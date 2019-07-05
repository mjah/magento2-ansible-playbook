# Magento 2 Ansible Playbook

This is an Ansible Playbook for Magento 2. It is used to set up a quick developer environment on a server.

**This is not recommended for production.**

It sets up a vanilla Magento 2 installation, and uses Nginx, MariaDB, and PHP.

This playbook was tested on Ubuntu 18.04 on a Digital Ocean node.

## Requirements

* Ubuntu 18.04 or similar environment
* Minimum 2GB RAM
* Root user access
* Magento access keys

## Installation

Update the values in:

* hosts
* group_vars/all.yml

Then after editing, run:

```sh
ansible-playbook -i hosts site.yml
```

## To-Do

* [ ] Ability to add custom PHP configuration.
* [ ] Create a **magento** linux user, instead of using root.
* [ ] (After magento user created) Set correct group permissions for magento installation.
* [ ] Set up magento_umask.
* [ ] Select version of Magento
