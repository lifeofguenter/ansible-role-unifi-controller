[![Build Status](https://travis-ci.org/lifeofguenter/ansible-role-unifi-controller.svg?branch=master)](https://travis-ci.org/lifeofguenter/ansible-role-unifi-controller)

# Ansible Role: UniFi Video

An Ansible role that installs UniFi Controller (Ubiquiti Networks) on Debian like systems.

## Requirements

none

## Role Variables

none

## Dependencies

- lifeofguenter.oracle-java

## Example Playbook

    - hosts: nvr
      roles:
        - { role: lifeofguenter.unifi-controller }

## License

MIT
