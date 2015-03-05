# dnsmasq\_proxy

A shared role for Ansible intended to provide painless setup of an internal
network DNS server that also acts as a proxy/cache for worldwide DNS lookups.

This is a very early release. At the moment, all it does is ensure that the
`dnsmasq` package is installed on systems that use `yum` or `pkgin` for their
package management.  In practical terms, that means it should be compatible
with all RedHat-class and SmartOS (Joyent) systems.

## Usage

Include something like what's below in your playbook.  (I think this is right;
I'm still an Ansible rookie.)

```yaml
- roles:
  - { role: "https://github.com/L2G/ansible-role-dnsmasq_proxy,,dnsmasq_proxy" }
```
