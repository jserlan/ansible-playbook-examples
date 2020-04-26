Webservers
==========

This role is using for deploying webservers with Apache HTTPd server running on Debian/Ubuntu.

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

For now, the settable variables are in the file vars/main.yml. Here we can custom the variables list "apache_common" used to install the common apache packages and "php_common" used to install the common php packages.

Example Playbook
----------------

Here an example of how to use this role :

    - hosts: servers
      roles:
         - role: webservers
