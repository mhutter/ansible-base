# ansible-base

Base setup for all my servers

**Q: What does it do?** A: See `tasks/`

## Getting started

- Have Ansible installed :open_mouth:
- Create a base playbook:

```yaml
---
- hosts: all
  roles:
    - base
```

- Example `hosts` file:

    [droplets]
    host1 ansible_ssh_host=1.2.3.4

- Example `~/.ansible.cfg` (or `/etc/ansible.cfg`):

    [defaults]
    remote_user = ansible

    [privilege_escalation]
    become = True
