# Ansible role for Varnish

This is a simple role that will install Varnish on Debian/Ubuntu from the stock APT repo.

## Sample playbook

```yaml
---

- hosts: myhost
  roles:
    - name: varnish
      tags: varnish
  vars:
    varnish_version: "6.2"
    varnishncsa_x_forwarded_for_enabled: true # if varnish is behind a reverse proxy
```
