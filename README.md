klems.sysadmin-tools
=========
[![Build Status](https://travis-ci.org/klems/ansible-role-sysadmin-tools.svg?branch=master)](https://travis-ci.org/klems/ansible-role-sysadmin-tools)

A role that allows you to install a pack of admin tools on a server

Requirements
------------
Ansible == `2.4`

Role Variables
--------------
### {{ sysadmin_tools }}
A list that contains all the sysadmin tools you want to install.

```
sysadmin_tools:
  - traceroute
  - telnet
  - netstat
  - nmap
```

Dependencies
------------
N/A

Example Playbook
----------------
```
- hosts: servers
  roles:
     - { role: klems.sysadmin-tools, sysadmin_tools: ['traceroute', 'telnet', 'netstat', 'nmap'] }
```

License
-------
BSD

Author Information
------------------
mail: klems@klems.net
