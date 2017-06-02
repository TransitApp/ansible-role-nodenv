# Ansible Role for Nodenv

[![Build Status](https://travis-ci.org/eventtus/ansible-role-nodenv.svg?branch=master)](https://travis-ci.org/eventtus/ansible-role-nodenv)
[![GitHub issues](https://img.shields.io/github/issues/eventtus/ansible-role-nodenv.svg?maxAge=2592000)](https://github.com/eventtus/ansible-role-nodenv/issues)

An Ansible role that installs Nodenv, NodeJS and node-build on Ubuntu and Debian

## Requirements

None

## Role Variables

### Defaults

    nodenv_user: "ubuntu"
    nodenv_path: ".nodenv"
    nodenv_version: "1.0.0"
    nodenv_default_version: "5.6.0"
    nodenv_versions:
    - 5.6.0

### Description

  - `nodenv_user`: System user to install nodenv for.
  - `nodenv_path`: Install path.
  - `nodenv_version`: Version of nodenv to install.
  - `nodenv_default_version`: The system's default version.
  - `nodenv_versions`: Array of versions of NodeJS to install.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
      - role: eventtus.nodenv
        nodenv_versions:
        - 5.6.0

## License

MIT/BSD

## Credits

[![Eventtus](http://assets.eventtus.com/logos/eventtus/standard.png)](http://eventtus.com)

Created by [Omar Abdel-Wahab](https://github.com/owahab) and sponsored by [Eventtus](http://eventtus.com).
