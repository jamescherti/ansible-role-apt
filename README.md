# ansible-role-apt
![License](https://img.shields.io/github/license/jamescherti/ansible-role-apt)

The [ansible-role-apt](https://github.com/jamescherti/ansible-role-apt) Ansible role manages the APT configuration and updates the `/etc/apt/sources.list` for Debian and Ubuntu systems.

## Role variables

Important variables:
| Variable               | Description                                                                                    | Default |
|------------------------|------------------------------------------------------------------------------------------------|---------|
| `apt_debian_community` | Enables community repositories (Debian *contrib* and *main*, or Ubuntu *universe*)             | true    |
| `apt_debian_nonfree`   | Enables non-free repositories (Debian *non-free*, *non-free-firmware*, or Ubuntu *multiverse*) | true    |
| `apt_debian_backports` | Enables the backports repository on Debian (no effect on Ubuntu systems)                       | false   |
| `apt_deb_src`          | Enables source package repositories (*deb-src* entries)                                        | false   |

Other variables:
| Variable                         | Description                | Default                                   |
|----------------------------------|----------------------------|-------------------------------------------|
| `apt_mirror_url_debian`          | Debian mirror URL          | `"http://deb.debian.org/debian"`          |
| `apt_mirror_url_debian_security` | Debian security mirror URL | `"http://deb.debian.org/debian-security"` |
| `apt_mirror_url_ubuntu`          | Ubuntu mirror URL          | `"http://archive.ubuntu.com/ubuntu"`      |

## Author and license

The *ansible-role-apt* role has been written by [James Cherti](https://www.jamescherti.com/) and is distributed under terms of the MIT license.

Copyright (C) 2000-2026 James Cherti

Distributed under terms of the MIT license.

# Links

- [ansible-role-apt @GitHub](https://github.com/jamescherti/ansible-role-apt)
