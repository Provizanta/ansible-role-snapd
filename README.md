Ansible role: snapd
=========

[![Build Status](https://travis-ci.com/Provizanta/ansible-role-snapd.svg?branch=master)](https://travis-ci.com/Provizanta/ansible-role-snapd)

Install and configure the snapd service (snap daemon).

Requirements
------------

None

Role variables
--------------

These variables can be defined:

    snapd_configuration: <dict, the entire daemon configuration in YAML format>

Dependencies
------------

None

Example Playbook
----------------

    - name: Converge
      hosts: all
      roles:
        - role: snapd
          vars:
            snapd_configuration:
              refresh:
                metered: "hold"
                timer: "sun5,20:00-23:00"
                retain: 2

License
-------

MIT

Author Information
------------------

Tibor Csóka
