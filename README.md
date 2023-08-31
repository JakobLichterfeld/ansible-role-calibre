# Ansible Role: Calibre

[![CI](https://github.com/JakobLichterfeld/ansible-role-calibre/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/JakobLichterfeld/ansible-role-calibre/actions/workflows/ci.yml)
[![Publish role on Ansible Galaxy](https://github.com/JakobLichterfeld/ansible-role-calibre/actions/workflows/publish_role_on_ansible_galaxy.yml/badge.svg?branch=main)](https://github.com/JakobLichterfeld/ansible-role-calibre/actions/workflows/publish_role_on_ansible_galaxy.yml)

Install Calibre via Binary Installer Download.

- Install dependencies
- Download Binary Installer Script
- Execute Binary Installer Script (optional: force update)

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

| Name           | Default Value   | Description                        |
| -------------- | --------------- | -----------------------------------|
| `calibre.force_update` | false | Whether to Force Update by executing the Installer every run |

## Dependencies

None.

## Example Playbook

```yaml
---
- hosts: all
  gather_facts: true
  become: true

  roles:
    - role: jakoblichterfeld.calibre
```

## License

MIT

## Author Information

This role was created in 2023 by [Jakob Lichterfeld](https://github.com/JakobLichterfeld).
