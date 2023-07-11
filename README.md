# lifeofguenter.unifi-controller

[![CircleCI](https://dl.circleci.com/status-badge/img/gh/lifeofguenter/ansible-role-unifi-controller/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/lifeofguenter/ansible-role-unifi-controller/tree/main)

An Ansible role that installs and configures a UniFi Controller on
Debian-like systems.

_**I do not recommend installing this role on systems but rather advise to use docker**_

## Requirements

none

## Role Variables

Available variables are listed below, along with default values:

```yaml
unifi_controller_jvm_xmx: 1024

mongodb_distribution_release: stretch|bionic # last supported with 3.6, can be installed on systems up to bullseye/focal
```

## Dependencies

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
