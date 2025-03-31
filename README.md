ansible-playbook-examples
=========================

Here are some examples of ansible playbooks that I use for my personnal projects

Directory structure
--------------------
    .
    ├── README copy.md
    ├── README.md
    ├── ansible.cfg
    ├── deploy-common.yml
    ├── deploy-webservers.yml
    ├── inventories
    │   └── hosts
    └── roles
        ├── common
        ├── ufw
        └── webservers

Folders content
---------------

inventories :
> contains the inventory files (hosts)

roles :
> contains all the role directory structures (common, ufw and webservers)

Files description
-----------------

README.md :
> this is the description file that your are currently reading ;)

ansible.cfg :
> this is the file that contains the parameters for the ansible. The parameters inside this file will overwrite the one in /etc/ansible/ansible.cfg

deploy-common.yml :
> this is the playbook used for deploying a common installation and configuration on the Debian/Ubuntu servers.

deploy-webservers.yml :
>this the playbook used for deploying the webservers with Apache HTTPd server running on Debian/Ubuntu.
