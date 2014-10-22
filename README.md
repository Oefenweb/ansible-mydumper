## mydumper

[![Build Status](https://travis-ci.org/Oefenweb/ansible-mydumper.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-mydumper) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-mydumper-blue.svg)](https://galaxy.ansible.com/list#/roles/1996)

Set up [mydumper](https://launchpad.net/mydumper) (How MySQL DBA & support engineer would imagine 'mysqldump') in Debian-like systems.

#### Requirements

* `libglib2.0-dev` (will be installed)
* `zlib1g-dev` (will be installed)
* `libpcre3-dev` (will be installed)
* `libmysqlclient18-dev` (will be installed)
* `libssl-dev` (will be installed)
* `python-sphinx` (will be installed)
* `cmake` (will be installed)
* `patch` (will be installed)

#### Variables

* `mydumper_version` [default: `{number: 0.6.2, url: https://launchpad.net/mydumper/0.6/0.6.2/+download/mydumper-0.6.2.tar.gz}`]: Version to install
* `mydumper_install_prefix` [default: `/usr/local`]: Install prefix (`cmake -DCMAKE_INSTALL_PREFIX`)

#### Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
  - mydumper
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-mydumper/issues)!
