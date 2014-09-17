## Docker Base: Apache


This repository contains **Dockerbase** of [Apache](http://httpd.apache.org/) for [Docker](https://www.docker.com/)'s [Dockerbase build](https://registry.hub.docker.com/u/dockerbase/apache/) published on the public [Docker Hub Registry](https://registry.hub.docker.com/).


### Depends on:

* [dockerbase/service](https://registry.hub.docker.com/u/library/service/)


### Installation

1. Install [Docker](https://docs.docker.com/installation/).

2. Download [Dockerbase build](https://registry.hub.docker.com/u/dockerbase/apache/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull dockerbase/apache`


### Usage

    run:
        sudo docker run --restart=always -t --cidfile cidfile -d dockerbase/apache /sbin/runit

    start:
        sudo docker start `cat cidfile`

    stop:
        sudo docker stop -t 10 `cat cidfile`

### Information
[Components & Versions](https://github.com/dockerbase/apache/blob/master/COMPONENTS)
