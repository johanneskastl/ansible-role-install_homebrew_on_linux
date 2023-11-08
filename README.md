![Ansible Lint](https://github.com/johanneskastl/ansible-role-install_homebrew_on_linux/workflows/Ansible%20Lint/badge.svg)

install_homebrew_on_linux
=========

Install the homebrew package manager on Linux (without running the bash
script).

Requirements
------------

None.

Role Variables
--------------

- `modify_bashrc_for_homebrew` (optional): If you want to modify the `.bashrc`
  to include the necessary statements for homebrew to work correctly, feel free
  to set this variable to `true`. It defaults to `false` and will not touch your
   `.bashrc`... :-)

Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: 'johanneskastl.install_homebrew_on_linux'
```

Example Playbook that modifies .bashrc
----------------

```yaml
- hosts: servers
  roles:
    - role: 'johanneskastl.install_homebrew_on_linux'
      modify_bashrc_for_homebrew: true
```

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via git@johannes-kastl.de.
