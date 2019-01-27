snapd
=========

snapd service (snap daemon).

Requirements
------------

None

Role 
--------------

Configuration file contents in YAML format.

    configuration: <dict, the entire configuration>

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

Tibor Csoka
