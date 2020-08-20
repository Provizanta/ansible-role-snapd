Ansible role: snapd
=========

![Build & Deploy](https://github.com/Provizanta/ansible-role-snapd/workflows/molecule/badge.svg?branch=master)

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
