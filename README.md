Ansible role: snapd
=========

Install and configure the snapd service (snap daemon).

Requirements
------------

None

Role variables
--------------

    configuration: <dict, the entire daemon configuration in YAML format>

Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      roles:
        - role: snapd
          vars:
            configuration:
              refresh:
                retain: 2

License
-------

MIT

Author Information
------------------

Tibor Csóka
