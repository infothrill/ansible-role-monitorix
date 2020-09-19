# Ansible role monitorix

[![Build Status](https://img.shields.io/travis/infothrill/ansible-role-monitorix/master.svg?label=travis_master)](https://travis-ci.org/infothrill/ansible-role-monitorix)
[![Build Status](https://img.shields.io/travis/infothrill/ansible-role-monitorix/develop.svg?label=travis_develop)](https://travis-ci.org/infothrill/ansible-role-monitorix)
[![Updates](https://pyup.io/repos/github/infothrill/ansible-role-monitorix/shield.svg)](https://pyup.io/repos/github/infothrill/ansible-role-monitorix/)
[![Ansible Role](https://img.shields.io/ansible/role/10800.svg)](https://galaxy.ansible.com/infothrill/monitorix/)

An [Ansible](http://www.ansible.com) role to install
[monitorix](http://www.monitorix.org/), a lightweight monitoring system on
Debian based Linux system.

## Quick howto

requirements.yml:

    - src: infothrill.monitorix
      version: v1.4.1

Install:

    ansible-galaxy install -r requirements.yml -p ./roles/

Playbook:

    - hosts: servers
        roles:
            - role: infothrill.monitorix

## Dependencies

No ansible dependencies.

## License

MIT

## Author Information

This role was created in 2016 by Paul Kremer.

## Changes

### v1.5.0

* Added support for ansible 2.8, 2.9
* Dropped support for python 2
* Dropped support for ansible `<=` 2.7
* Dropped support for ubuntu 14 LTS
* Added support for ubuntu 20 LTS, Debian Buster

### v1.4.1

* dropped support for Debian wheezy
* updated molecule,docker and ansible-lint

### v1.4.0

* upgraded docker driver
* updated monitorix default version

### v1.3.2

* upgraded docker driver

### v1.3.1

* fixed test execution

### v1.3.0

* added ansible 2.7 support
* dropped ansible 2.4 support (EOL)

### v1.2

* dropped ansible 2.2 and 2.3 support (EOL)

### v1.1

* upgraded monitorix minor version in defaults
* added ansible 2.5 test
* dropped ansible 2.1 tests
* upgraded molecule

### v1.0

* initial release
