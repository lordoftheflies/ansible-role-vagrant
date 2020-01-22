---
title: 'ansible-role-vagrant'
description: 'Vagrant manager role.'
feedback: true
comments: true
---

# Ansible Role: Vagrant

Management role for Vagrant.

### Vagrant

Vagrant is a tool for building and managing virtual machine environments in a single workflow. With an easy-to-use workflow and focus on automation, Vagrant lowers development environment setup time, increases production parity, and makes the "works on my machine" excuse a relic of the past.

## Requirements

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

## Role Variables

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

## Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

## Usage

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yml
    - hosts: servers
      roles:
         - { role: lordoftheflies.ansibale_role_vagrant, x: 42 }
```

Local installation : (ansible need to be installed)

```bash
git clone git@gitlab.cherubits.hu:oss/ansible-galaxy-roles/ansible-role-vagrant.git
ansible-playbook -i "localhost," --ask-sudo-pass --connection=local installation.yml
```

Simple Usage :
```yml
---
 - hosts: all
   roles:
    - vagrant
```

Usage with version specification
```yml
---
 - hosts: all
   roles:
    - role: vagrant
      vagrant_version: "1.6.3"
```

Specify virtualbox installation (For Debian)
```yml
---
 - hosts: all
   roles:
    - role: vagrant
      vagrant_virtualbox_install: True
      vagrant_virtualbox_ver: "virtualbox-5.1"
```

## License

Apache-2.0

## Author Information

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
