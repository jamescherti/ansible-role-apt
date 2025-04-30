# ansible-role-apt
![License](https://img.shields.io/github/license/jamescherti/ansible-role-apt)

An Ansible role that manages the APT configuration and updates the `/etc/apt/sources.list` for Debian and Ubuntu systems.

## Role variables

Important variables:
| Variable                     | Description                           | Default                              |
|------------------------------|---------------------------------------|--------------------------------------|
| `apt_community`              | Enable community repositories         | true                                 |
| `apt_nonfree`                | Enable non-free repositories          | true                                 |
| `apt_debian_backports`       | Enable backports repository on Debian | false                                |


Other variables:
| Variable                     | Description                | Default                                   |
|------------------------------|----------------------------|-------------------------------------------|
| `apt_mirror_debian`          | Debian mirror URL          | `"http://deb.debian.org/debian"`          |
| `apt_mirror_debian_security` | Debian security mirror URL | `"http://deb.debian.org/debian-security"` |
| `apt_mirror_ubuntu`          | Ubuntu mirror URL          | `"http://archive.ubuntu.com/ubuntu"`      |
| `apt_mirror_release`         | Release codename           | `{{ ansible_distribution_release }}`      |

## Author and license

The *ansible-role-apt* role has been written by [James Cherti](https://www.jamescherti.com/) and is distributed under terms of the MIT license.

Copyright (C) 2000-2025 James Cherti

Distributed under terms of the MIT license.

# Links

- [ansible-role-apt @GitHub](https://github.com/jamescherti/ansible-role-apt)
