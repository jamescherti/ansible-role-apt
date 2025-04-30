# ansible-role-apt-sources-list
![License](https://img.shields.io/github/license/jamescherti/ansible-role-apt-sources-list)

This ansible role manages the APT proxy configuration and updates the `/etc/apt/sources.list` for Debian and Ubuntu systems. It optionally configures community and non-free repositories and supports backports on Debian.

## Role variables

| Variable                     | Description                           | Required | Default                              |
|------------------------------|---------------------------------------|----------|--------------------------------------|
| `apt_proxy`                  | Proxy URL for APT                     | No       | ""                                   |
| `apt_mirror`                 | Debian mirror URL                     | Yes      | `"http://deb.debian.org"`            |
| `apt_mirror_debian`          | Debian mirror URL                     | Yes      | `"{{ apt_mirror }}/debian"`          |
| `apt_mirror_debian_security` | Debian security mirror URL            | Yes      | `"{{ apt_mirror }}/debian-security"` |
| `apt_mirror_ubuntu`          | Ubuntu mirror URL                     | Yes      | `"{{ apt_mirror }}/ubuntu"`          |
| `apt_mirror_release`         | Release codename                      | Yes      | `{{ ansible_distribution_release }}` |
| `apt_community`              | Enable community repositories         | No       | true                                 |
| `apt_nonfree`                | Enable non-free repositories          | No       | true                                 |
| `apt_debian_backports`       | Enable backports repository on Debian | No       | false                                |

## Author and license

The *ansible-role-apt-sources-list* role has been written by [James Cherti](https://www.jamescherti.com/) and is distributed under terms of the MIT license.

Copyright (C) 2000-2025 James Cherti

Distributed under terms of the MIT license.

# Links

- [ansible-role-apt-sources-list @GitHub](https://github.com/jamescherti/ansible-role-apt-sources-list)
