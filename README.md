bind-consul
=========

Configures DNS forwarding for Consul using bind and iptables.

Requirements
------------

 * Consul
 * Bind
 * Systemd
 * iptables

Role Variables
--------------

    bind_consul_inventory_group: bind_consul
    bind_consul_nameserver: 127.0.0.1
    bind_consul_nameserver_port: 8600

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

Steve Verhelle (enqack) enqack@gmail.com
