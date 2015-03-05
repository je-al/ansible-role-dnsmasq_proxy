dnsmasq\_proxy
==============

This Ansible role is meant to provide painless setup of an internal
network DNS server that also acts as a proxy/cache for worldwide DNS lookups.

This is a very early release. At the moment, all it does is ensure that the
`dnsmasq` package is installed on systems that use `yum` or `pkgin` for their
package management.  In practical terms, that means it should be compatible
with all RedHat-class and SmartOS (Joyent) systems.

Requirements
------------

See above

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

    - hosts: internal\_dns\_servers
      roles:
         - { role: L2G.dnsmasq_proxy }

License
-------

Creative Commons Attribution 4.0 International (http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

Larry "Lawrence Leonard" Gilbert, larry@L2G.to, https://github.com/L2G, 844-L2G-GEEK
