[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)
[![Build Status](https://travis-ci.org/LIP-Computing/ansible-role-os-cli.svg?branch=master)](https://travis-ci.org/LIP-Computing/ansible-role-os-cli)

LIP-Computing.ansible-role-os-cli
=================================

The role deploys the Openstack CLI

Role Variables
--------------

There are no role variables

Example Playbook
----------------

The directory tests/os-cli.yml provide an example of playbook

    - hosts: localhost
      roles:
         - LIP-Computing.ansible-role-os-cli

Docker images
-------------

The directory docker contains Dockerfiles for Ubuntu 16.04 and for Cento7.

The images are in dockerhub and automatically built from this repository:

* https://hub.docker.com/r/lipcomputing/os-cli-centos7/
* https://hub.docker.com/r/lipcomputing/os-cli-ubuntu16.04/

License
-------

Apache v2

Author Information
------------------

Mario David: <mariojmdavid@gmail.com>

LIP Lisbon: http://www.lip.pt

Indigo DataCloud: https://www.indigo-datacloud.eu/
