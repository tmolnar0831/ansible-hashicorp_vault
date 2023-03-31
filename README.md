hashicorp_vault
=========

A simple Ansible role that installs Hashicorp Vault on Debian Linux

Requirements
------------

This role tries to be as simple as it is possible. The only requirement is an installed Ansible 2.9+ to use it.

Role Variables
--------------

Every variable here has default values handled in the "defaults". The role is written for Debian Bullseye.

```
vault_gpg_url: https://apt.releases.hashicorp.com/gpg

vault_apt_repo: deb https://apt.releases.hashicorp.com $(lsb_release -cs) main

vault_install_packages:
  - vault
```

Dependencies
------------

This role tries to be as simple as it is possible. The only requirement is an installed Ansible to use it.

Example Playbook
----------------

Just include it in the roles and all set.

    - hosts: all
      roles:
         - role: hashicorp_vault

License
-------

MIT

Author Information
------------------

Tamas Molnar - <tmolnar0831@gmail.com> - https://tomsitcafe.com
