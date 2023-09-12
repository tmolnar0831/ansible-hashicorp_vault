hashicorp_vault
=========

This is an Ansible role that installs Hashicorp Vault on Debian Linux

Requirements
------------

- Ansible >= 2.10

Role Variables
--------------

```
vault_gpg_url: https://apt.releases.hashicorp.com/gpg
vault_apt_repo: deb https://apt.releases.hashicorp.com bookworm main
vault_install_packages:
  - vault
```

Dependencies
------------

- Ansible >= 2.10

Example Playbook
----------------

    - hosts: all
      roles:
         - role: hashicorp_vault

License
-------

MIT

Author Information
------------------

Tamas Molnar - <tmolnar0831@gmail.com> - https://tomsitcafe.com
