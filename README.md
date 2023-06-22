# ansible-role-orchestrator #

[![GitHub Build Status](https://github.com/cisagov/ansible-role-orchestrator/workflows/build/badge.svg)](https://github.com/cisagov/ansible-role-orchestrator/actions)
[![CodeQL](https://github.com/cisagov/ansible-role-orchestrator/workflows/CodeQL/badge.svg)](https://github.com/cisagov/ansible-role-orchestrator/actions/workflows/codeql-analysis.yml)

An Ansible role for installing
[cisagov/orchestrator](https://github.com/cisagov/orchestrator).

## Requirements ##

None.

## Role Variables ##

| Variable | Description | Default | Required |
|----------|-------------|---------|----------|
| file_owner_group | The name of the group that should own any files or directories created by this role. | [Omitted](https://docs.ansible.com/ansible/latest/user_guide/playbooks_filters.html#making-variables-optional) | No |
| file_owner_username | The name of the user that should own any files or directories created by this role. | [Omitted](https://docs.ansible.com/ansible/latest/user_guide/playbooks_filters.html#making-variables-optional) | No |

## Dependencies ##

- [cisagov/ansible-role-docker](https;//github.com/cisagov/ansible-role-docker)

## Example Playbook ##

Here's how to use it in a playbook:

```yaml
- hosts: docker
  become: yes
  become_method: sudo
  tasks:
    - name: Install the BOD 18-01 scanning orchestrator composition
      ansible.builtin.include_role:
        name: orchestrator
```

## Contributing ##

We welcome contributions!  Please see [`CONTRIBUTING.md`](CONTRIBUTING.md) for
details.

## License ##

This project is in the worldwide [public domain](LICENSE).

This project is in the public domain within the United States, and
copyright and related rights in the work worldwide are waived through
the [CC0 1.0 Universal public domain
dedication](https://creativecommons.org/publicdomain/zero/1.0/).

All contributions to this project will be released under the CC0
dedication. By submitting a pull request, you are agreeing to comply
with this waiver of copyright interest.

## Author Information ##

Shane Frasier - <jeremy.frasier@gwe.cisa.dhs.gov>
