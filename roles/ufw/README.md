UFW
===

This role is used for deploying ufw installation and configuration on Debian/Ubuntu.

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

For now, there is only one usable variables that is public_ports. This variable is a list of variables  and is used to allow remote access to public ports on the servers. If the variable is undefined, the task will be ignored. The variable can be set when the role is include inside a playbook.

Example Playbook
----------------

Here's an example of how to use this role and how the variable can be passed as parameters:

    - hosts: servers
      roles:
         - { role: ufw, public_ports: [8080] }
