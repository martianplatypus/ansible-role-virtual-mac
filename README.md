virtual-mac
=========

[![Galaxy Role][badge-role]][link-galaxy]
[![Build Status][badge-travis]][link-travis]
[![MIT Licensed][badge-license]][link-license]

Uses homebrew to install VirtualBox, Vagrant and Vagrant-manager on MacOS 10.13 and above.

Requirements
------------

VirtualBox and Vagrant are installed via brew cask.

Hombrew can be installed using the following command in a terminal:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

Alternatively, you can install homebrew using this role:
```
ansible-galaxy install geerlingguy.homebrew
```

Role Variables
--------------

A list of casks to be installed:
```
homebrew_cask_apps
```
* virtualbox
* virtualbox-extension-pack
* vagrant
* vagrant-manager

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: localhost
      roles:
         - role: ansible-role-virtual-mac


[badge-role]: https://img.shields.io/ansible/role/47242.svg?style=flat-square
[badge-license]: https://img.shields.io/github/license/martianplatypus/ansible-role-virtual-mac
[badge-travis]: https://img.shields.io/travis/com/martianplatypus/ansible-role-virtual-mac
[link-galaxy]: https://galaxy.ansible.com/martianplatypus/virtual_mac/
[link-license]: https://github.com/martianplatypus/ansible-role-virtual-mac/blob/master/LICENSE
[link-travis]: https://travis-ci.com/github/martianplatypus/ansible-role-virtual-mac/
