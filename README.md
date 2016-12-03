Ansible Role: Franz
=========

[![Build Status](https://travis-ci.org/patrick-hill/ansible-role-franz.svg?branch=master)](https://travis-ci.org/patrick-hill/ansible-role-franz)


Install [Franz](http://meetfranz.com/) chat client and drops the .desktop file for the Start Menu.

Requirements
------------

Ansible 1.6+

Role Variables
--------------


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: localhost
      gather_facts: yes
      roles:
         - role: patrick-hill.conky

*Inside `defaults/main.yml`*:

    conky_use_backup: true

License
-------

BSD

Author Information
------------------

Role written in 2016 by [Patrick Hill](http://www.HillsPCWorld.com) 
