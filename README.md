Role Name
=========
This role will install ansible on redhar and debian machines

Requirements
------------

 you should have at-leat one control machine with ansible install :)

Role Variables
--------------
ansible_ver: 2.0.1.0

prereq_ubuntu:
    - software-properties-common
    - python-pip
    - python-dev

prereq_redhat:
    - python-pip
    - python-setuptools
    - openssl-devel
    - python-devel

pipreq:
    - paramiko
    - PyYAML
    - Jinja2
    - httplib2
    - six



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: cnighojkar.ansible, ansible_ver: 2.0.0.1 }

License
-------

BSD
