firewalld
=====

This role installs and configures firewalld.

Examples:

```
firewalld_default_zone: home

firewalld_zone_interface:
  home: eno1

firewalld_service_rules: 
  mdns:
    state: enabled
    zone: home
    permanent: yes
    immediate: yes
  ipp-client:
    state: enabled
    zone: home
    permanent: yes
    immediate: yes
  dhcpv6-client:
    state: enabled
    zone: home
    permanent: yes
    immediate: yes
  samba-client:
    state: enabled
    zone: home
    permanent: yes
    immediate: yes
```