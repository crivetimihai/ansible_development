Ansible Development Collection
==============================

[Ansible Galaxy Collection: Development](https://galaxy.ansible.com/crivetimihai/development):

- anaconda: install anaconda (miniconda) and various packages from conda / pip
- cloudcli - install various cloud CLIs (aws, helm, azure, oc, kubectl, ibmcloud, etc.)

Tested on:
----------

- CentOS 7
- RHEL 8
- Fedora 30
- Ubuntu 18.04
- Debian 10

Example
-------

### Install the role:

```bash
pip install --upgrade mazer
mazer install crivetimihai.development
```


### playbook.yml example

```yaml
- name: setup a development environment
  hosts: all
  connection: local
  become: yes
  gather_facts: yes
  roles:
    - role: crivetimihai.development.anaconda
```

# See also:

- [Ansible Virtualization Collection](https://galaxy.ansible.com/crivetimihai/virtualization)
- [Ansible Workstation Collection](https://github.com/crivetimihai/ansible_workstation)
- [Ansible Server Collection](https://github.com/crivetimihai/ansible_server)
- [Ansible CookieCutter Collection and Role Template with Molecule](https://github.com/crivetimihai/ansible_cookiecutter)
