# ansible-role-orchestrator #

[![Build Status](https://travis-ci.com/cisagov/ansible-role-orchestrator.svg?branch=develop)](https://travis-ci.com/cisagov/ansible-role-orchestrator)
[![Total alerts](https://img.shields.io/lgtm/alerts/g/cisagov/ansible-role-orchestrator.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/cisagov/ansible-role-orchestrator/alerts/)
[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/cisagov/ansible-role-orchestrator.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/cisagov/ansible-role-orchestrator/context:python)

An Ansible role for installing
[cisagov/orchestrator](https://github.com/cisagov/orchestrator).

## Requirements ##

None.

## Role Variables ##

None.

## Dependencies ##

None.

## Example Playbook ##

Here's how to use it in a playbook:

```yaml
- hosts: docker
  become: yes
  become_method: sudo
  roles:
    - orchestrator
```

## Contributing ##

We welcome contributions!  Please see [here](CONTRIBUTING.md) for
details.

## License ##

This project is in the worldwide [public domain](LICENSE.md).

This project is in the public domain within the United States, and
copyright and related rights in the work worldwide are waived through
the [CC0 1.0 Universal public domain
dedication](https://creativecommons.org/publicdomain/zero/1.0/).

All contributions to this project will be released under the CC0
dedication. By submitting a pull request, you are agreeing to comply
with this waiver of copyright interest.

## Author Information ##

First Last - <first.last@trio.dhs.gov>
