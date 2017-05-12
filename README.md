## Golang

[![Ansible Galaxy](http://img.shields.io/badge/galaxy-DimitriSteyaert/golang-660198.svg?style=flat)](https://galaxy.ansible.com/detail#/role/DimitriSteyaert)


This role basically just installs the Go programming language on your system.

### Installation

This role requires at least Ansible `v1.9`. To install it, run:

```Shell
ansible-galaxy install DimitriSteyaert/golang
```


### Role variables

List of default variables available in the inventory:

```YAML
---
go_version: 1.8.1
go_checksum: 'sha256:a579ab19d5237e263254f1eac5352efcf1d70b9dacadb6d6bb12b0911ede8994'
go_parentdir: /usr/local
```


### Detailed usage guide

By default version 1.8.1 is installed but you can define the version of your choice, just don't forget to define the correct checksum for the version you define. This installation goes into the parent directory /usr/local but this parameter can also be modified.
Upgrading or downgrading of Go on your system can be done by defining another `go_version`.

#### Examples

This is a basic playbook to install Go with the default variables:
```YAML
---
- hosts: all
  roles:
    - golang
```

### Authors and license

The `golang` role was written by:

- [Dimitri Steyaert](https://www.steyaert.be) | [e-mail](mailto:dimitri@steyaert.be) | [Twitter](https://twitter.com/DimitriSteyaert)

License: [MIT](https://tldrlegal.com/license/mit-license)

***

README generated by [Ansigenome](https://github.com/nickjj/ansigenome/).
