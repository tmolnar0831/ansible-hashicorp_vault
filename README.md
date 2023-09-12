hashicorp_vault
=========

This is an Ansible role that installs Hashicorp Vault on Debian Linux using APT.

HashiCorp Vault is an open-source tool designed for managing secrets and protecting sensitive data within modern infrastructure and applications. It provides a secure and centralized way to store, access, and distribute secrets such as API keys, passwords, certificates, and other sensitive information. HashiCorp Vault helps organizations achieve data security and compliance by offering features like encryption, access control, auditing, and dynamic secret generation.

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
