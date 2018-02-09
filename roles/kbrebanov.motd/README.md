motd
====

[![Build Status](https://travis-ci.org/kbrebanov/ansible-motd.svg?branch=master)](https://travis-ci.org/kbrebanov/ansible-motd)

Generate MOTD file.

Requirements
------------

This role requires Ansible 1.9 or higher.

Role Variables
--------------

| Name            | Default                           | Description                               |
|:----------------|:----------------------------------|:------------------------------------------|
| motd_ascii_logo | ""                                | ASCII logo to be displayed before message |
| motd_message    | Welcome to {{ ansible_hostname }} | MOTD message                              |

Dependencies
------------

None

Example Playbook
----------------

Generate MOTD file using default ASCII logo and message.
```yaml
- hosts: all
  roles:
    - kbrebanov.motd
```

Generate MOTD file using default ASCII logo and custom message.
```yaml
- hosts: all
  vars:
    motd_message: This is the new message
  roles:
    - kbrebanov.motd
```

License
-------

BSD

Author Information
------------------

Kevin Brebanov
