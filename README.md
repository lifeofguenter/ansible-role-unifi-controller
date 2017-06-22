[![Build Status](https://travis-ci.org/lifeofguenter/ansible-role-unifi-controller.svg?branch=master)](https://travis-ci.org/lifeofguenter/ansible-role-unifi-controller)

# Ansible Role: UniFi controller

An Ansible role that installs UniFi Controller (Ubiquiti Networks) on Debian like systems.

## Requirements

none

## Role Variables

- `unifi_controller_jvm_xmx: 1024M`
- `unifi_user: unifi`

## Dependencies

- lifeofguenter.oracle-java

## Example Playbook

    - hosts: gw
      roles:
        - { role: lifeofguenter.unifi-controller }

## License

MIT
