ansible-role-ohmyzsh
=========

<p align="center">

<a href="https://github.com/iancleary/ansible-role-ohmyzsh/actions?query=workflow%3Aci" target="_blank">
    <img src="https://github.com/iancleary/ansible-role-ohmyzsh/workflows/CI/badge.svg" alt="CI workflow status">
</a>

<a href="https://github.com/iancleary/ansible-role-ohmyzsh/actions?query=workflow%3Arelease" target="_blank">
    <img src="https://github.com/iancleary/ansible-role-ohmyzsh/workflows/Release/badge.svg" alt="Release workflow status">
</a>

<a href="https://raw.githubusercontent.com/iancleary/ansible-role-ohmyzsh/main/LICENSE" target="_blank">
    <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
</a>
</p>

This role installs zsh, ohmyzsh, ohmyzsh plugins, custom ohmyzsh plugins, and custom ohmyzsh themes.

Requirements
------------

None

Role Variables
--------------


Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- hosts: servers
  user: unprivelaged
  roles:
    - role: iancleary.ohmyzsh
```

**Note the underscore in `ohmyzsh`, it is not a dash!**

> This role doesn't need to be run as root, use whatever user you want to clone the repos as.

```yaml
- hosts: servers
  user: root
  roles:
    - role: iancleary.ohmyzsh
```

> Note: `"- role: geerlingguy.git"` is only there to ensure `git` is installed.  You may remove that line, if `git` is installed by some other method.

License
-------

[MIT](LICENSE)

Author Information
------------------

This role was created in 2023 by [Ian Cleary](https://iancleary.me).

Inspiration for the structure of this repo came from [Jeff Geerling](https://github.com/geerlingguy/ansible-role-nginx).
