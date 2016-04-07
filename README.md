Role Name: sardpost.elasticsearch
=================================
Ansible role for installing Elasticsearch 2.x on EL 7 platform (RHEL/Centos 7).
The role installs the repo and elasticsearch 2.x.

Requirements
------------
Oracle Java JDK 8 installed
Platform: RHEL/Centos 7


Dependencies
------------
Java. Any role that provides Java the latest version (8). Example:
```yml
   - sardpost.java8
```

Example Playbook
----------------
```yml
  - name: Install Elasticsearch
    hosts: test_lab
    remote_user: centos
    sudo: yes

    roles:
      - sardpost.java8
      - sardpost.elasticsearch
```
Version:
--------
0.1

License
-------
GPLv3

Author Information
------------------
Davide M. Puggioni
