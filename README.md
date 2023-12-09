# lifeofguenter.unifi-controller

[![CircleCI](https://dl.circleci.com/status-badge/img/gh/lifeofguenter/ansible-role-unifi-controller/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/lifeofguenter/ansible-role-unifi-controller/tree/main)

An Ansible role that installs and configures a UniFi Controller on
Debian-like systems.

## Compatability Matrix

| UniFi Controller Version | OS             | Java | MongoDB |
|--------------------------|----------------|------|---------|
| <7.5                     | Debian Stretch | 11   | 3.6     |
| 7.5+                     | Ubuntu 20.04   | 17   | 4.4     |

## Requirements

none

## Role Variables

Available variables are listed below, along with default values:

```yaml
unifi_controller_jvm_xmx: 1024

unifi_release: stable # unifi-7.5
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
