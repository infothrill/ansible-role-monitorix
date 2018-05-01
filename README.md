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
	  version: v1.1

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

### v1.1

* upgraded monitorix minor version in defaults
* added ansible 2.5 test
* dropped ansible 2.1 tests
* upgraded molecule

### v1.0

* initial release

