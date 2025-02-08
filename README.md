chrony
======
[![Ansible Lint](https://github.com/oxivanisher/role-chrony/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/oxivanisher/role-chrony/actions/workflows/ansible-lint.yml)

This role installs and configured chrony for time synchronization.

Role Variables
-----------

| Name                | Comment                              | Default value |
|---------------------|--------------------------------------|---------------|
| chrony_ntp_servers  | Ntp servers to be used | `0.ch.pool.ntp.org`, `1.ch.pool.ntp.org`, `2.ch.pool.ntp.org`, `3.ch.pool.ntp.org`         |


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
- name: Configure ntp
  hosts: all
  collections:
    - oxivanisher.linux_base
  roles:
    - role: oxivanisher.linux_base.chrony
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.linux_base](https://galaxy.ansible.com/ui/repo/published/oxivanisher/linux_base/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-linux_base).
