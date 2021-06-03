# Ansible Role: UniFi controller

[![Build Status](https://travis-ci.com/lifeofguenter/ansible-role-unifi-controller.svg?branch=main)](https://travis-ci.com/lifeofguenter/ansible-role-unifi-controller)

An Ansible role that installs UniFi Controller (Ubiquiti Networks) on Debian like systems.

## Requirements

none

## Role Variables

- `unifi_controller_jvm_xmx: 1024M`
- `unifi_user: unifi`

## Dependencies

- [lifeofguenter.java](https://galaxy.ansible.com/lifeofguenter/java)

## Example Playbook

    - hosts: gw
      roles:
        - { role: lifeofguenter.unifi_controller }

## License

MIT
