## mydumper

[![Build Status](https://travis-ci.org/Oefenweb/ansible-mydumper.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-mydumper) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-mydumper-blue.svg)](https://galaxy.ansible.com/list#/roles/0)

Set up [mydumper](https://launchpad.net/mydumper) (How MySQL DBA & support engineer would imagine 'mysqldump') in Debian-like systems.

#### Requirements

None

#### Variables

* `mydumper_version` [default: `{number: 0.6.2, url: https://launchpad.net/mydumper/0.6/0.6.2/+download/mydumper-0.6.2.tar.gz}`]: Version to install

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
