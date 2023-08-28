# Ansible Role: Calibre

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
  gather_facts: yes
  become: true

  roles:
    - role: jakoblichterfeld.calibre
```

## License

MIT

## Author Information

This role was created in 2023 by [Jakob Lichterfeld](https://github.com/JakobLichterfeld).
