
# Ansible Role: OpenStack Ansible Zaqar 0.1


An Ansible Role to deploy OpenStack Zaqar on Ubuntu LTS 

This is an unofficial prototype for an independant role for use with the 
[OpenStack Ansible](http://governance.openstack.org/reference/projects/openstackansible.html) 
project. See also the project page on the 
[OpenStack Wiki](https://wiki.openstack.org/wiki/OpenStackAnsible) and the project 
[repository on Github](https://github.com/openstack/openstack-ansible).

## Requirements

This role assumes you have an OpenStack deploy which conforms to the architectural model 
described in the OpenStack Ansible project, as well as a MongoDB server which is managed
independently. 

## Role Variables

TBD

## Dependencies

This role relies on three roles from the OpenStack Ansible project: memcached, openrc, and 
pip_lock_down which will need to be symlinked or otherwise made available in a way that 
allows Ansible to locate them.

## Example Playbook

    - hosts: zaqar_containers
      roles:
        - { role: stevelle.openstack-ansible-zaqar }

## License

Apache 2.0