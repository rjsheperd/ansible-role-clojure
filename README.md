# Ansible Role: Clojure

[![Build Status](https://travis-ci.org/paginagmbh/ansible-role-clojure.svg?branch=master)](https://travis-ci.org/paginagmbh/ansible-role-clojure)

An Ansible Role that installs [Clojure](https://clojure.org/) on Linux.

## Requirements

A Java runtime has to be installed on the target host.

## Example Playbook

``` yaml
- role: geerlingguy.java
- role: gremid.clojure
```

## Tests

To run the test playbook(s):

  1. Install and start Docker.
  1. Download the test shim (see .travis.yml file for the URL) into `tests/test.sh`:
  1. Make the test shim executable: `chmod +x tests/test.sh`.
  1. Run (from the role root directory) `distro=[distro] playbook=[playbook] ./tests/test.sh`

If you don't want the container to be automatically deleted after the test playbook is run, add the following environment variables:

    cleanup=false container_id=$(date +%s)

## License

BSD

## Author Information

This role was created in 2018 by [Pagina GmbH](https://www.pagina.gmbh/).

It draws heavily from best practices as demonstrated in roles authored by [Jeff Geerling](https://www.jeffgeerling.com/), author of [Ansible for DevOps](https://www.ansiblefordevops.com/).
