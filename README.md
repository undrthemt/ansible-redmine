Ansible-Redmine
====

## Overview

Redmine server's script for ansible.

rails + mysql + apache + passenger


## Description
Install redmine on centos 6 server.

ruby on rails with rbenv, mysql database, apache web server,and passenger.

Redmine will be installed by ansible_ssh_user.


<br>
This script is just only install redmine with it's dependencies. 

If you want to setup redmine on public server, please be secure.
Make sure iptables, SE Linux, apache conf files, and permissions of files.

## Requirement
Support OS CentOS 6.

ansible version 1.9.6 or later.

## Usage
- Configure hosts file for your servers.
- Configure group_vars/all file.
- Configure playbooks/redmine.yml file.
- Edit roles/ruby/vars/main.yml file, if want to change ruby version.

<br>
Then run the playbook.

```
ansible-playbook playbooks/redmine.yml -i hosts
```

- Change redmine admin user's password.

## Licence

[MIT](https://opensource.org/licenses/mit-license.php)

