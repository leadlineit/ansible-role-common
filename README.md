# Ansible Galaxy role for install common packages.

![Build Status](https://github.com/leadlineit/ansible-role-common/actions/workflows/ansible-galaxy-ci.yml/badge.svg)
[![Galaxy Role](https://img.shields.io/badge/Ansible--Galaxy-leadlineit.common-blue.svg?logo=ansible&logoColor=white)](https://galaxy.ansible.com/leadlineit/common/)

This role helps to install common packages.

Supported OSes
--------------
- Debian 12 (bookworm)
- Debian 11 (bullseye)
- Debian 10 (buster)
- Debian 9 (stretch)

Requirements
------------

This role requires Ansible 2.11 or higher.

Role Variables
--------------

The role have only one variable.
So, you can add any package you want to install, like this (for example):

```yaml
---
common_packages:
  - apt-transport-https
  - bash-completion
  - ca-certificates
  - curl
  - git
  - gnupg2
  - htop
  - iftop
  - iotop
  - mc
  - ncdu
  - pigz
  - screen
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
