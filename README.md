bind-consul
=========

Configures DNS forwarding for Consul using bind and iptables.

Requirements
------------

 * Consul
 * Bind
 * iptables

Role Variables
--------------

    bind_consul_inventory_group: bind_consul
    bind_consul_consul_address: 127.0.0.1
    bind_consul_consul_dns_port: 8600

Example Playbook
----------------

Host file:

    [nameservers]
    ns1.example.com
    ns2.example.com
    ns1.example.net
    ns2.example.net

    [bind_consul]
    ns1.example.net
    ns2.example.net


Playbook:

    - hosts: nameservers
      roles:
         - role: enqack.bind-consul

License
-------

BSD

Author Information
------------------

Steve Verhelle (enqack) enqack@gmail.com
