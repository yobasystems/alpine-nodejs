# nodejs Docker image running on Alpine Linux

[![Docker Layers](https://img.shields.io/badge/docker%20layers-2-blue.svg?maxAge=2592000?style=flat-square)](https://hub.docker.com/r/yobasystems/alpine-nodejs/) [![Docker Size](https://img.shields.io/badge/docker%20size-17%20MB-blue.svg?maxAge=2592000?style=flat-square)](https://hub.docker.com/r/yobasystems/alpine-nodejs/) [![Docker Stars](https://img.shields.io/docker/stars/yobasystems/alpine-nodejs.svg?maxAge=2592000?style=flat-square)](https://hub.docker.com/r/yobasystems/alpine-nodejs/) [![Docker Pulls](https://img.shields.io/docker/pulls/yobasystems/alpine-nodejs.svg?maxAge=2592000?style=flat-square)](https://hub.docker.com/r/yobasystems/alpine-nodejs/)

[![Alpine Version](https://img.shields.io/badge/alpine%20version-v3.8.0-green.svg?maxAge=2592000?style=flat-square)](http://alpinelinux.org/) [![nodejs Version](https://img.shields.io/badge/nodejs%20LTS%20version-v8.11.3-green.svg?maxAge=2592000?style=flat-square)](https://nodejs.org/) [![NPM Version](https://img.shields.io/badge/NPM%20version-v5.6.0-green.svg?maxAge=2592000?style=flat-square)](http://npm.org)


This Docker image [(yobasystems/alpine-nodejs)](https://hub.docker.com/r/yobasystems/alpine-nodejs/) is based on the minimal [Alpine Linux](http://alpinelinux.org/) with [Node.js LTS](https://nodejs.org/).

##### Alpine Version 3.8.0 (Released June 26, 2018)
##### Node.js Version 8.11.3
##### NPM Version 5.6.0

----

## What is Alpine Linux?
Alpine Linux is a Linux distribution built around musl libc and BusyBox. The image is only 5 MB in size and has access to a package repository that is much more complete than other BusyBox based images. This makes Alpine Linux a great image base for utilities and even production applications. Read more about Alpine Linux here and you can see how their mantra fits in right at home with Docker images.

## What is Node.js?
Node.js is a platform built on Chrome's JavaScript runtime for easily building fast and scalable network applications. Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient, perfect for data-intensive real-time applications that run across distributed devices.

## Features

  * Minimal size only
    * 17 MB and only 2 layers
    * 13 MB and only 2 layers :min version (Nodejs v6.10.3)
    * 20 MB and only 2 layers :current version (Nodejs v8.6.0)
  * Memory usage is minimal on a simple install.
  * Nodejs LTS Version 6.11.3
  * NPM Version 3.10.10

## Architectures

* ```:amd64```, ```:latest``` - 64 bit Intel/AMD (x86_64/amd64)
* ```:i386```, ```:x86``` - 32 bit Intel/AMD (x86/i686)
* ```:arm64v8```, ```:aarch64``` - 64 bit ARM (ARMv8/aarch64)
* ```:arm32v7```, ```:armhf``` - 32 bit ARM (ARMv7/armhf)

#### PLEASE CHECK TAGS BELOW FOR SUPPORTED ARCHITECTURES, THE ABOVE IS A LIST OF EXPLANATION

## Tags

* ```:latest```, ```:amd64``` latest branch based on amd64 (LTS Version of nodejs)
* ```:master``` master branch usually inline with latest
* ```:min``` latest branch with alpine package version
* ```:current``` latest branch with latest version of nodejs
* ```:v0.0.0``` version number related to docker version
* ```:armhf```, ```:arm32v7``` Armv7 based on latest tag but arm architecture
* ```:armhf-min```, ```:arm32v7-min``` Armv7 based on latest tag but arm architecture and includes alpine package version
* ```:armhf-current```, ```:arm32v7-current``` Armv7 based on latest tag but arm architecture and includes latest node.js

## Creating an instance

```docker run yobasystems/alpine-nodejs```

or

```docker run yobasystems/alpine-nodejs:min```


## Source Repository

* [Bitbucket - yobasystems/alpine-nodejs](https://bitbucket.org/yobasystems/alpine-nodejs/)

* [Github - yobasystems/alpine-nodejs](https://github.com/yobasystems/alpine-nodejs)

## Links

* [Yoba Systems](https://www.yobasystems.co.uk/)

* [Dockerhub - yobasystems](https://hub.docker.com/u/yobasystems/)

* [Quay.io - yobasystems](https://quay.io/organization/yobasystems)
