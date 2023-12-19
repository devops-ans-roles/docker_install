Docker Install
=========

This Ansible role installs Docker Engine on Ubuntu-based virtual machines. It's designed to make the installation of Docker on multiple machines as straightforward as possible.


Requirements
------------

Thi role is specifically developed for Ubuntu-based systems. While it may work on other Debian-based distributions, it has not been tested on them.

Role Variables
--------------

The role uses variables which can be found in `defaults/main.yml`. You can override these variables in your playbook if necessary.

Dependencies
------------

No other Ansible roles are required for this role.

Example Playbook
----------------

Here's an example playbook `docker_install.yml` using this role:

```yaml
---
- name: Install Docker Engine
  hosts: all
  become: true
  roles:
    - docker_install`
```


To use this playbook, ensure your Ansible inventory file is set up correctly with the hosts you want to target.

