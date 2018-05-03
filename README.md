## mydumper

[![Build Status](https://travis-ci.org/Oefenweb/ansible-mydumper.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-mydumper) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-mydumper-blue.svg)](https://galaxy.ansible.com/tersmitten/mydumper)

Set up [mydumper](https://github.com/maxbube/mydumper) (How MySQL DBA & support engineer would imagine 'mysqldump') in Debian-like systems.

#### Requirements

* `libglib2.0-dev` (will be installed)
* `zlib1g-dev` (will be installed)
* `libpcre3-dev` (will be installed)
* `libmysqlclient-dev` (will be installed)
* `libssl-dev` (will be installed)
* `python-sphinx` (will be installed)
* `build-essential` (will be installed)
* `cmake` (will be installed)
* `patch` (will be installed)

#### Variables

* `mydumper_version` [default: `{number: 0.9.3, url: https://github.com/maxbube/mydumper/archive/v0.9.3.tar.gz}`]: Version to install
* `mydumper_install_prefix` [default: `/usr/local`]: Install prefix (`cmake -DCMAKE_INSTALL_PREFIX`)
* `mydumper_libmysqlclient_dev` [default: `libmysqlclient-dev`]: `libmysqlclient-dev` version to install. Percona Server users might want to change this to `libperconaserverclient16-dev` (5.1), `libperconaserverclient18-dev` (5.5), `libperconaserverclient18.1-dev` (5.6) or `libperconaserverclient20-dev` (5.7).

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
