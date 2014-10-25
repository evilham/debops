## [![DebOps project](http://debops.org/images/debops-small.png)](http://debops.org) apt

[![Travis CI](http://img.shields.io/travis/debops/ansible-apt.svg?style=flat)](http://travis-ci.org/debops/ansible-apt) [![test-suite](http://img.shields.io/badge/test--suite-ansible--apt-blue.svg?style=flat)](https://github.com/debops/test-suite/tree/master/ansible-apt/)  [![Ansible Galaxy](http://img.shields.io/badge/galaxy-debops.apt-660198.svg?style=flat)](https://galaxy.ansible.com/list#/roles/1551)

`debops.apt` configures and manages APT package manager in Debian and other
derivative distributions. Specifically, it will manage:

* list of APT sources
* centralized APT cache (using `apt-cacher-ng`)
* automatic package updates (using `unattended-upgrades` and `apticron`)
* Debian Preseed configuration
* local APT repository (using `reprepro`)
* installation of custom packages specified in Ansible inventory

### Installation

This role requires at least Ansible `v1.7.0`. To install it, run:

    ansible-galaxy install debops.apt

### Documentation

More information about `debops.apt` can be found in the
[official debops.apt documentation](http://docs.debops.org/en/latest/ansible/roles/debops.apt.html).


### Role dependencies

- `debops.etc_services`
- `debops.nginx`
- `debops.reprepro`
- `debops.ferm`
- `debops.apt_preferences`
- `debops.secret`

### Are you using this as a standalone role without DebOps?

You may need to include missing roles from the [DebOps common
playbook](https://github.com/debops/debops-playbooks/blob/master/playbooks/common.yml)
into your playbook.

[Try DebOps now](https://github.com/debops/debops) for a complete solution to run your Debian-based infrastructure.





### Authors and license

`apt` role was written by:
- Maciej Delmanowski | [e-mail](mailto:drybjed@gmail.com) | [Twitter](https://twitter.com/drybjed) | [GitHub](https://github.com/drybjed)

License: [GPLv3](https://tldrlegal.com/license/gnu-general-public-license-v3-%28gpl-3%29)

***

This role is part of the [DebOps](http://debops.org/) project. README generated by [ansigenome](https://github.com/nickjj/ansigenome/).
