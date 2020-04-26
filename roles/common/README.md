Common
======

This role is using for deploying a common installation and configuration on Debian/Ubuntu.

Directory structure
--------------------

    .
    ├── README.md
    ├── defaults
    ├── files
    ├── handlers
    ├── tasks
    ├── templates
    └── vars

Role Variables
--------------

For now, the settable variables are in the file vars/main.yml. Here we can custom the variables list "monitoring_tools", "admin_tools" and "utils" used to install the monintoring packages, the admin tools packages and any utils packages. The variables locale allow you to define the locale used on the servers and timezone allow you to define the timezone for your region.

Example Playbook
----------------

Here an example of how to use this role :

    - hosts: servers
      roles:
         - role: common
