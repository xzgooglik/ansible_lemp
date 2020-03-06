Ansible LEMP
==================
- nginx latest
- php 7.0/7.1/7.2/7.3/7.4
- mysql 5.7

Installation
------------

Platforms
---------

Supports all platforms:

Amazon Linux 2
CentOS versions: 6, 7 
Debian versions: 9 (stretch), 10 (buster)

Variables
--------------
This role has multiple variables. Package  variables are located in group_vars/all


Run Playbook (nginx: latest, php: 7.3, percona-mysql: 5.7) 
----------------------------------------------------------

$ ansible-playbook lemp.yml

Run Playbook using another package version:
----------------------------------------------------------
 - php: 7.0/7.1/7.2/7.3/7.4
 - mysql: 5.7 (percona-mysql 8.0 - in the future)

$ ansible-playbook lemp.yml -e php_ver=7.2 mysql_ver=5.7



Author Information
------------------

[Dmitry Chernov](https://github.com/amiDMast)
