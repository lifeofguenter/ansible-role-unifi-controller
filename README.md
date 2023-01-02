# lifeofguenter.unifi-controller

[![Build Status](https://travis-ci.com/lifeofguenter/ansible-role-unifi-controller.svg?branch=main)](https://travis-ci.com/lifeofguenter/ansible-role-unifi-controller)

An Ansible role that installs and configures a UniFi Controller on
Debian-like systems.

_I do not recommend installing this role on systems but rather advise to use docker._

## Requirements

none

## Role Variables

Available variables are listed below, along with default values:

```yaml
unifi_controller_jvm_xmx: 1024

mongodb_distribution_release: bionic|stretch
```

## Dependencies

- [lifeofguenter.java](https://galaxy.ansible.com/lifeofguenter/java)
- [lifeofguenter.monogdb](https://galaxy.ansible.com/lifeofguenter/mongodb)

## Example Playbook

```yaml
- hosts: gw
  roles:
    - { role: lifeofguenter.unifi_controller }
```
## License

**MIT**, see the [LICENSE file](LICENSE) for details.

## Author Information

[Günter Grodotzki](https://www.lifeofguenter.de)
