# os-cli-ubuntu16.04
[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)

Docker image with ansible based on the lipcomputing/docker-ansible-centos7

## Installed packages

Base:
- Ansible

Image specific:
- Openstack CLI

## Build

```bash
docker build --rm -t os-cli-centos7 .
```

## Usage

```bash
$ docker run -it os-cli-centos7 /bin/bash
```

You should set the Openstack variables:

```bash
export OS_PROJECT_DOMAIN_NAME=default
export OS_USER_DOMAIN_NAME=default
export OS_PROJECT_NAME=<Project Name>
export OS_USERNAME=<Username>
export OS_PASSWORD=<Password>
export OS_AUTH_URL=<Keystone auth endpoint>
export OS_IDENTITY_API_VERSION=3
export OS_IMAGE_API_VERSION=2
```

```bash
# openstack image list
```

License
-------

Apache v2

Author Information
------------------

Mario David: <mariojmdavid@gmail.com>

LIP Lisbon: http://www.lip.pt

Indigo DataCloud: https://www.indigo-datacloud.eu/

