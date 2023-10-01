FROM yobasystems/alpine:3.18.3-amd64

ARG BUILD_DATE
ARG VCS_REF

LABEL maintainer="Dominic Taylor <dominic@yobasystems.co.uk>" \
    architecture="amd64/x86_64" \
    nodejs-version="min" \
    alpine-version="3.18.3" \
    build="01-Oct-2023" \
    org.opencontainers.image.title="alpine-nodejs" \
    org.opencontainers.image.description="Nodejs container image running on Alpine Linux" \
    org.opencontainers.image.authors="Dominic Taylor <dominic@yobasystems.co.uk>" \
    org.opencontainers.image.vendor="Yoba Systems" \
    org.opencontainers.image.version="min" \
    org.opencontainers.image.url="https://hub.docker.com/r/yobasystems/alpine-nodejs/" \
    org.opencontainers.image.source="https://github.com/yobasystems/alpine-nodejs" \
    org.opencontainers.image.revision=$VCS_REF \
    org.opencontainers.image.created=$BUILD_DATE

RUN apk add --no-cache nodejs npm
