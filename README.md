# ansible-role-apt
![License](https://img.shields.io/github/license/jamescherti/ansible-role-apt)

This ansible role manages the APT proxy configuration and updates the `/etc/apt/sources.list` for Debian and Ubuntu systems.

## Role variables

| Variable                     | Description                           | Required | Default                              |
|------------------------------|---------------------------------------|----------|--------------------------------------|
| `apt_proxy`                  | Proxy URL for APT                     | No       | ""                                   |
| `apt_mirror`                 | Debian mirror URL                     | Yes      | `"http://deb.debian.org"`            |
| `apt_community`              | Enable community repositories         | No       | true                                 |
| `apt_nonfree`                | Enable non-free repositories          | No       | true                                 |
| `apt_debian_backports`       | Enable backports repository on Debian | No       | false                                |

## Author and license

The *ansible-role-apt* role has been written by [James Cherti](https://www.jamescherti.com/) and is distributed under terms of the MIT license.

Copyright (C) 2000-2025 James Cherti

Distributed under terms of the MIT license.

# Links

- [ansible-role-apt @GitHub](https://github.com/jamescherti/ansible-role-apt)
