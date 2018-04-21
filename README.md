# Ansible role monitorix

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

