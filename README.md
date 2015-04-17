Ansible role to install Ruby and Bundler
=======================================

Use this role to install Ruby from source in /usr/local/ on Debian based systems. After installing Ruby it will also install Bundler, so users of the system can install their dependencies in a local bundler directory.

Usage
-----
Add this role in your playbook. Optionally override `ruby_version` and `ruby_sha256` to install a different version.
