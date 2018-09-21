# Ansible Role: sysctl

Manipulates sysctl entries.

[https://manpages.debian.org/stretch/procps/sysctl.8.en.html](https://manpages.debian.org/stretch/procps/sysctl.8.en.html)

# Role Variables

sysctl_entries: []

# Example Playbook

```
- hosts: server
  vars:
    sysctl_entries:
      - { key: 'fs.file-max', value: 1048576 }
  roles:
    - { role: honomoa.sysctl }
```

# License
CC BY-SA 3.0
