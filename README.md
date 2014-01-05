Ansible apt
===========

Basic roles for apt management in Ansible.

Examples:

Update package information.
Use in depencies of roles instaling packages `meta/main.yml`.

    dependencies:
      - { role: "apt/update" }

Upgrade all packages to last version:

    roles:
      - "apt/upgrade"

Define apt proxy for instalation:

    vars:
      apt_proxy_server: "http://aptproxy.lan:3142"
    roles:
      - "apt/proxy"

Requirements
------------

Linux system with apt package management (Debian, Ubuntu).

Dependencies
------------

None

License
-------

BSD

Author Information
------------------

Michael Heča
