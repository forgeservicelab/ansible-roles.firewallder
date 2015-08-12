Firewallder
===========

Configures CentOS firewalld daemon's zones and services.

Requirements
------------

Configuration files are not provided.
Both zone and service configuration files are XML files according to firewalld documentation

Role Variables
--------------

- `services_dir` - Path of the directory containing service configuration files. If relative, starting at `files` (see [Looping over fileglobs](http://docs.ansible.com/playbooks_loops.html#looping-over-fileglobs))
- `zones_dir` - Path of the directory containing zone configuration files.
- `default_zone` - Default zone for the firewall. Defaults to `public`.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - role: firewallder
          services_dir: /home/user/configs/services
          zones_dir: /home/user/configs/zones


License
-------

MIT

Author Information
------------------

FORGE ServiceLab team.
