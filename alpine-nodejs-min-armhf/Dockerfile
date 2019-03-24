FROM yobasystems/alpine:3.9.2-armhf

ARG BUILD_DATE
ARG VCS_REF

LABEL maintainer="Dominic Taylor <dominic@yobasystems.co.uk>" \
    architecture="arm32v7/armhf" \
    nodejs-version="min" \
    alpine-version="3.9.2" \
    build="24-Mar-2019" \
    org.opencontainers.image.title="alpine-nodejs" \
    org.opencontainers.image.description="Nodejs Docker image running on Alpine Linux" \
    org.opencontainers.image.authors="Dominic Taylor <dominic@yobasystems.co.uk>" \
    org.opencontainers.image.vendor="Yoba Systems" \
    org.opencontainers.image.version="min" \
    org.opencontainers.image.url="https://hub.docker.com/r/yobasystems/alpine-nodejs/" \
    org.opencontainers.image.source="https://github.com/yobasystems/alpine-nodejs" \
    org.opencontainers.image.revision=$VCS_REF \
    org.opencontainers.image.created=$BUILD_DATE

RUN apk add --no-cache nodejs nodejs-npm
