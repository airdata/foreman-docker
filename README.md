Foreman 1.16
-------------
This is a foreman in docker is with ec2 and docker plugin.

[![MIT Licensed](http://img.shields.io/badge/license-MIT-green.svg)](https://tldrlegal.com/license/mit-license)
[![Automated Build](https://img.shields.io/docker/build/dock0/foreman.svg)](https://hub.docker.com/r/airdata/foreman-docker/)
[![CircleCI](https://img.shields.io/circleci/project/github/airdata/foreman-in-docker.svg)](https://circleci.com/gh/airdata/foreman-in-docker) 

Requierments to running this image is to start container with a hostname - foreman.lab.

Run container
========================

```
docker run -d -h foreman.lab airdata/foreman-docker
```

docker-compose
===============
```
git clone https://github.com/airdata/foreman-docker.git && \
 cd foreman-docker && \
 docker-compose up -d
```

Persistent Volumes 
==================

Running container in with persistent volumes for to avoiding losing data:

 ```
 /var/lib/postgresql:/var/lib/postgresql
 /etc/puppetlabs/code:/etc/puppetlabs/code
 /opt/puppetlabs:/opt/puppetlabs
```
