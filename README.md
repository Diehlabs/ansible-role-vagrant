# ansible-role-vagrant
[![Ansible Lint](https://github.com/Diehlabs/ansible-role-vagrant/actions/workflows/test.yml/badge.svg)](https://github.com/Diehlabs/ansible-role-vagrant/actions/workflows/test.yml)
=========

This role will install Vagrant and optionally VirtualBox.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

Defaults:
| Variable name | Description | Example value | Default value | Required? |
|---|---|---|---|---|
| vagrant_install_hyperv | Intall Hyper-V, only affects Windows targets | True | False | NO |
| vagrant_vbox_version | Version of VirtualBox to install | 6.1 | 6.1 | YES |
| vagrant_vbox | Misc options | [See defaults](defaults/main.yml) | -- | YES |

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - { role: ansible-role-vagrant, vagrant_vbox_version: 5.0 }

License
-------

MIT

Author Information
------------------

[Chris Diehl](https://www.linkedin.com/in/chrisdiehl817/)
