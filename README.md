# Ansible Role : EyesOfNetwork

Deploy last EyesOfNetwork version on a CentOS 7.4 host.

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
      version: 5
      release: 2
```

Author Information
------------------

* **Jean-Philippe Levy** - *Initial work* - [EyesOfNetwork Community](https://github.com/eyesofnetworkcommunity)
