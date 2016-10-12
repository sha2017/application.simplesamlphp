Role Name
=========

SimpleSAMLphp, install either as SP or IdP. Currently based on Debian distro.

Requirements
------------

- Debian
- Nginx / php

Role Variables
--------------

* **ssp_task** Install either as Service Provider or Identity Provider
* **ssp_base_url** Main public url your host is reachable, no / at the end
* more to come

Example Playbook
----------------

    - name: SimpleSAMLphp
      hosts: simplesamlhost
      vars:
        - ssp_task: sp
        - ssp_base_url: "https://service.mydomain.com"
      roles:
       - simplesamlphp

TODO
----

- Alot! This is first draft...
- Conditionals checking
- Make distro agnostic
- Make the IdP setup work
- Finish this document

License
-------

BSD

Author
------
Peter Tambach, piele@sha2017.org
