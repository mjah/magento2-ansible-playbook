# Magento 2 Ansible Playbook

**In-Progress**

This is an Ansible Playbook for Magento 2. It is used to set up a quick developer environment on a server. This is not recommended for production.

## Requirements

* Ubuntu 18.04
* Root user access

## Usage

Update the values in:

* hosts
* group_vars/all.yml

Then after editing, run:

```sh
ansible-playbook -i hosts site.yml
```
