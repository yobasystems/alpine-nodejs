FROM yobasystems/alpine:3.21.1-aarch64

ARG BUILD_DATE
ARG VCS_REF

LABEL maintainer="Dominic Taylor <dominic@yoba.systems>" \
    architecture="arm64v8/aarch64" \
    nodejs-version="min" \
    alpine-version="3.21.1" \
    build="29-Jan-2025" \
    org.opencontainers.image.title="alpine-nodejs" \
    org.opencontainers.image.description="Nodejs container image running on Alpine Linux" \
    org.opencontainers.image.authors="Dominic Taylor <dominic@yoba.systems>" \
    org.opencontainers.image.vendor="Yoba Systems" \
    org.opencontainers.image.version="min" \
    org.opencontainers.image.url="https://hub.docker.com/r/yobasystems/alpine-nodejs/" \
    org.opencontainers.image.source="https://github.com/yobasystems/alpine-nodejs" \
    org.opencontainers.image.base.name="docker.io/yobasystems/alpine:3.21.1" \
    org.opencontainers.image.revision=$VCS_REF \
    org.opencontainers.image.created=$BUILD_DATE

RUN addgroup -g 1000 node \
    && adduser -u 1000 -G node -s /bin/sh -D node \
    && apk add --no-cache nodejs npm
