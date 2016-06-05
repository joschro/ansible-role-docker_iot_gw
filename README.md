ROLE-NAME
==========

Ansible role to set up an IoT gateway in a docker container.

Requirements
------------
A host running the Docker service and a base image, e.g. created with https://github.com/joschro/ansible-role-docker_base_image .

Role Variables
--------------

None.

Dependencies
------------

None.

Example Playbook
----------------
```
- name: NAME
  hosts: dockerhosts
  remote_user: root

  roles:
    - ROLE
```
with an inventory file like this for example:
```
[dockerhosts]
dockerhost ansible_ssh_host=<above-ip-address> ansible_ssh_user=root
```

License
-------

GPLv3

Author Information
------------------

Joachim Schröder, jos (at) redhat.com
