# Ansible Role: TrueNAS SCALE Web Interface QOL Patch

This Ansible role applies a patch to the TrueNAS SCALE web interface for quality of life improvements.

## Installation

```bash
ansible-galaxy role install Panzer1119.truenas-scale-web-interface-qol-patch
```

## Variables

- `uncolor_storage_dashboard_topology_warning_icons`: Whether to uncolor storage dashboard topology warning icons (default: `true`)

## Example Playbook

```yaml
- hosts: all
  become: yes
  vars:
    uncolor_storage_dashboard_topology_warning_icons: true
  roles:
    - Panzer1119.truenas-scale-web-interface-qol-patch
```

Test it with the following command:

```bash
ansible-playbook -i inventory playbook.yml -CD
```
