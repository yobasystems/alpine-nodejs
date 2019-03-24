# nodejs Docker image running on Alpine Linux

[![Docker Automated build](https://img.shields.io/docker/automated/yobasystems/alpine-nodejs.svg?style=for-the-badge&logo=docker)](https://hub.docker.com/r/yobasystems/alpine-nodejs/)
[![Docker Pulls](https://img.shields.io/docker/pulls/yobasystems/alpine-nodejs.svg?style=for-the-badge&logo=docker)](https://hub.docker.com/r/yobasystems/alpine-nodejs/)
[![Docker Stars](https://img.shields.io/docker/stars/yobasystems/alpine-nodejs.svg?style=for-the-badge&logo=docker)](https://hub.docker.com/r/yobasystems/alpine-nodejs/)

[![Alpine Version](https://img.shields.io/badge/Alpine%20version-v3.9.2-green.svg?style=for-the-badge)](https://alpinelinux.org/)
[![nodejs Version](https://img.shields.io/badge/nodejs%20LTS%20version-v10.15.3-green.svg?style=for-the-badge)](https://nodejs.org/)
[![NPM Version](https://img.shields.io/badge/NPM%20version-v6.4.1-green.svg?style=for-the-badge)](https://npm.org)


This Docker image [(yobasystems/alpine-nodejs)](https://hub.docker.com/r/yobasystems/alpine-nodejs/) is based on the minimal [Alpine Linux](https://alpinelinux.org/) with [Node.js LTS](https://nodejs.org/).

##### Alpine Version 3.9.2 (Released March 04, 2019)
##### Node.js Version 10.15.3
##### NPM Version 6.4.1

----

## What is Alpine Linux?
Alpine Linux is a Linux distribution built around musl libc and BusyBox. The image is only 5 MB in size and has access to a package repository that is much more complete than other BusyBox based images. This makes Alpine Linux a great image base for utilities and even production applications. Read more about Alpine Linux here and you can see how their mantra fits in right at home with Docker images.

## What is Node.js?
Node.js is a platform built on Chrome's JavaScript runtime for easily building fast and scalable network applications. Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient, perfect for data-intensive real-time applications that run across distributed devices.

## Features

* Minimal size only
* Memory usage is minimal on a simple install

## Architectures

* ```:amd64```, ```:x86_64``` - 64 bit Intel/AMD (x86_64/amd64)
* ```:arm64v8```, ```:aarch64``` - 64 bit ARM (ARMv8/aarch64)
* ```:arm32v7```, ```:armhf``` - 32 bit ARM (ARMv7/armhf)

##### PLEASE CHECK TAGS BELOW FOR SUPPORTED ARCHITECTURES, THE ABOVE IS A LIST OF EXPLANATION

## Tags

* ```:latest``` latest branch based on lts nodejs (Automatic Architecture Selection)
* ```:min``` package branch with alpine package version installed from alpine repos (Automatic Architecture Selection)
* ```:current``` current branch with latest bleeding edge current version of nodejs (Automatic Architecture Selection)
* ```:v0.0.0``` version number related to node.js version (Automatic Architecture Selection)
* ```:amd64```, ```:x86_64```  amd64 based on latest tag but amd64 architecture
* ```:min-amd64```, ```:min-x86_64```  amd64 based on latest tag but amd64 architecture and includes alpine package version
* ```:current-amd64```, ```:current-x86_64```  amd64 based on latest tag but amd64 architecture and includes current node.js
* ```:armhf```, ```:arm32v7``` Armv7 based on latest tag but arm32 architecture latest branch based on lts node.js
* ```:min-armhf```, ```:min-arm32v7``` Armv7 based on latest tag but arm architecture and includes alpine package version
* ```:current-armhf```, ```:current-arm32v7``` Armv7 based on latest tag but arm architecture and includes current node.js
* ```:aarch64```, ```:arm64v8``` Armv8 based on latest tag but arm64 architecture latest branch based on lts node.js
* ```:min-aarch64-min```, ```:min-arm64v8``` Armv8 based on latest tag but arm64 architecture and includes alpine package version
* ```:current-aarch64```, ```:current-arm64v8``` Armv8 based on latest tag but arm64 architecture and includes current node.js

## Layers & Sizes

![Version](https://img.shields.io/badge/version-amd64-blue.svg?style=for-the-badge)
![MicroBadger Layers (tag)](https://img.shields.io/microbadger/layers/yobasystems/alpine-nodejs/amd64.svg?style=for-the-badge)
![MicroBadger Size (tag)](https://img.shields.io/microbadger/image-size/yobasystems/alpine-nodejs/amd64.svg?style=for-the-badge)

![Version](https://img.shields.io/badge/version-aarch64-blue.svg?style=for-the-badge)
![MicroBadger Layers (tag)](https://img.shields.io/microbadger/layers/yobasystems/alpine-nodejs/aarch64.svg?style=for-the-badge)
![MicroBadger Size (tag)](https://img.shields.io/microbadger/image-size/yobasystems/alpine-nodejs/aarch64.svg?style=for-the-badge)

![Version](https://img.shields.io/badge/version-armhf-blue.svg?style=for-the-badge)
![MicroBadger Layers (tag)](https://img.shields.io/microbadger/layers/yobasystems/alpine-nodejs/armhf.svg?style=for-the-badge)
![MicroBadger Size (tag)](https://img.shields.io/microbadger/image-size/yobasystems/alpine-nodejs/armhf.svg?style=for-the-badge)

## Creating an instance

```docker run yobasystems/alpine-nodejs```

or

```docker run yobasystems/alpine-nodejs:min```

or

```docker run yobasystems/alpine-nodejs:current```


## Source Repository

* [Bitbucket - yobasystems/alpine-nodejs](https://bitbucket.org/yobasystems/alpine-nodejs/)

* [Github - yobasystems/alpine-nodejs](https://github.com/yobasystems/alpine-nodejs)

## Links

* [Yoba Systems](https://www.yobasystems.co.uk/)

* [Dockerhub - yobasystems](https://hub.docker.com/u/yobasystems/)

* [Quay.io - yobasystems](https://quay.io/organization/yobasystems)
