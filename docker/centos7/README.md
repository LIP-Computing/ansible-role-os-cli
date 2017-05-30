[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)
[![](https://images.microbadger.com/badges/image/lipcomputing/os-cli-centos7.svg)](http://microbadger.com/images/lipcomputing/os-cli-centos7 "Get your own image badge on microbadger.com")

# os-cli-centos7

Docker image with ansible based on the lipcomputing/ansible-centos7

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


Run the image in dockerhub and mounting a directory contained the openstack
shell scripts with environment variables:

```bash
docker run -it --privileged -v `pwd`:/home lipcomputing/os-cli-centos7 /bin/bash
```

License
-------

Apache v2

Author Information
------------------

Mario David: <mariojmdavid@gmail.com>

LIP Lisbon: http://www.lip.pt

Indigo DataCloud: https://www.indigo-datacloud.eu/

