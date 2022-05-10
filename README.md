# Ansible Galaxy role for install common Debian packages.

![Build Status](https://github.com/leadlineit/ansible-role-common/actions/workflows/ansible-galaxy-ci.yml/badge.svg)
[![Galaxy Role](https://img.shields.io/badge/Ansible--Galaxy-leadlineit.common-blue.svg?logo=ansible&logoColor=white)](https://galaxy.ansible.com/leadlineit/common/)

This role helps to install common packages to Debian (stretch/buster/bullseye).

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

The role have only one variable.
So, you can add any package you want to install, like this (for example):

```yaml
---
common_packages:
  - iotop
  - htop
  - iftop
  - screen 
  - mc
  - curl
  - bash-completion 
  - apt-transport-https
  - ca-certificates
  - gnupg2
  - git
  - pigz
  - ncdu
```

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- hosts: servers
  roles:
    - { role: leadlineit.common, tags: common }
```

License
-------

BSD

Author Information
------------------

This role was created by Stas Stavnichuk.
