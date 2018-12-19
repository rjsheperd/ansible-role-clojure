# Ansible Role: Clojure

[![Build Status](https://travis-ci.org/paginagmbh/ansible-role-clojure.svg?branch=master)](https://travis-ci.org/paginagmbh/ansible-role-clojure)

An Ansible Role that installs [Clojure](https://clojure.org/) on Linux.

## Requirements

A Java runtime has to be installed on the target host.

## Example Playbook

``` yaml
# Register EPEL repo for 'rlwrap' package on RH distros
- role: geerlingguy.repo-epel
  when: ansible_os_family == "RedHat"
- role: geerlingguy.java
- role: gremid.clojure
```

## License

BSD

## Author Information

This role was created in 2018 by [Pagina GmbH](https://www.pagina.gmbh/).

It draws heavily from best practices as demonstrated in roles authored by [Jeff Geerling](https://www.jeffgeerling.com/), author of [Ansible for DevOps](https://www.ansiblefordevops.com/).
