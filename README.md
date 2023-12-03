Setup Linux Environment
=======================

A role for setting up linux environment. Currently used for ubuntu 23/22

## Features

- Installs zsh + antigen. See variable zsh_

Requirements
------------

To setup a dev environment and run molecule, install poetry.

### Install Poetry

[https://python-poetry.org/docs/#installation](https://python-poetry.org/docs/#installation)

### Install environment using poetry

Run inside directory: `poetry install`

Role Variables
--------------

```
stplin_zsh_antigen_bundles: []
```

Dependencies
------------

- viasite-ansible.zsh

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: souldiv.setup_linux_vm
            vars:
                 zsh_user: test

License
-------

BSD
