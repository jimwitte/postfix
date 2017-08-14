jimwitte.postfix
================
postfix configured for sending email notifications. Forward email from root to a "real" email account. install mailutils.

Requirements
------------
tested with Ubuntu 16.04.

Role Variables
--------------
* postfix_admin_email: "myemail@example.com"
* postfix_inet_interfaces: "loopback-only"

override these in your playbook or change them in vars/main.yml

Example Playbook
----------------
    - hosts: all
      roles:
         - { role: postfix, tags: ['postfix'] }
