Ansible role to install Ruby and Bundler
=======================================

Use this role to install Ruby from source in /usr/local/ on Debian based systems or using the package manager on OpenBSD. After installing Ruby it will also install Bundler, so users of the system can install their dependencies in a local bundler directory.

Requirements
------------

This role will work on Debian based systems and OpenBSD.

Role Variables
--------------

Optionally override `ruby_version` and `ruby_sha256` to install a different ruby version.

Dependencies
------------

None.

Example Playbook
----------------

The following playbook will install Ruby 2.1.6 instead of the role defined version.

    - hosts: servers
      vars:
        - ruby_version: 2.1.6
        - ruby_sha256: 1e1362ae7427c91fa53dc9c05aee4ee200e2d7d8970a891c5bd76bee28d28be4
      roles:
         - ivaldi.ruby

License
-------

BSD

Author Information
------------------

Developed by Frank Groeneveld for use by [Ivaldi](http://ivaldi.nl/).
