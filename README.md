# Ansible Role : EyesOfNetwork

Ansible Role for EyesOfNetwork.

Requirements
------------

CentOS 7.4 with minimal install.

Role Variables
--------------

* `version` - EyesOfNetwork version (default 5)
* `release` - EyesOfNetwork release (deafult 2)

Example Playbook
----------------

```
- name: Install EyesOfNetwork Monitoring 
  hosts: eyesofnetwork
  remote_user: root
  tasks:
  - import_role:
      name: eyesofnetwork
      tasks_from: install
    vars:
      eon_version: 5
      eon_release: 2
```

Author Information
------------------

* **Jean-Philippe Levy** - <jean-philippe.levy@axians.com> - [EyesOfNetwork Community](https://github.com/eyesofnetworkcommunity)
