Ansible Role: Franz
=========

[![Build Status](https://travis-ci.org/patrick-hill/ansible-role-franz.svg?branch=master)](https://travis-ci.org/patrick-hill/ansible-role-franz)


Install [Franz](http://meetfranz.com/) chat client and drops the .desktop file for the Start Menu.

Requirements
------------

Ansible 2.1+

Role Variables
--------------

    franz_version: 4.0.4
"franz_version" is the version of Franz to install

    franz_download_link: https://github.com/meetfranz/franz-app/releases/download/{{ franz_version }}/Franz-linux-x64-{{ franz_version }}.tgz
"franz_download_link" can be overridden if need be but just update the version above 

    franz_create_desktop_file: true
"franz_create_desktop_file" creates the menu entry in the Start Menu

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: localhost
      gather_facts: yes
      roles:
         - role: patrick-hill.franz

*Inside `defaults/main.yml`*:

    franz_version: 4.0.4
    franz_download_link: https://github.com/meetfranz/franz-app/releases/download/{{ franz_version }}/Franz-linux-x64-{{ franz_version }}.tgz
    franz_create_desktop_file: true

License
-------

BSD

Author Information
------------------

Role written in 2016 by [Patrick Hill](http://www.HillsPCWorld.com) 
