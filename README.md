# ansible-base

Base setup for my servers :rocket:

**Q: What does it do?** A: See `tasks/`

## Getting started

Base playbook example:

```yaml
---
- hosts: all
  roles:
    - base
```

Example `hosts` file:

    [droplets]
    host1 ansible_ssh_host=1.2.3.4

Example `~/.ansible.cfg` (or `/etc/ansible.cfg`):

    [defaults]
    remote_user = ansible

    [privilege_escalation]
    become = True
