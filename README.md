ansible-role-route53
====================

Ansible role to handle route53 without ansible route53 module

Requirements
------------

installed and working aws cli

Role Variables
--------------

    aws_route53_record: some_route.example.org

Record which should be updated (no default value)

    aws_route53_zone: example.org

Zone which should be used to perform the update (no default value)

    aws_ip: 127.0.0.1

IP which should be set for the record (do default value)
If no IP ist set, then this role uses metadata to discover an IP 

    aws_route53_ttl: 3600

TimeToLive for the record in seconds (default: 3600)


Dependencies
------------

none

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: solutionDrive.route53

License
-------

MIT

Author Information
------------------

solutionDrive <technik@solutiondrive.de>
