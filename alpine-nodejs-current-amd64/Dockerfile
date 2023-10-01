FROM yobasystems/alpine:3.18.3-amd64

ARG BUILD_DATE
ARG VCS_REF

LABEL maintainer="Dominic Taylor <dominic@yobasystems.co.uk>" \
    architecture="amd64/x86_64" \
    nodejs-version="current" \
    alpine-version="3.18.3" \
    build="01-Oct-2023" \
    org.opencontainers.image.title="alpine-nodejs" \
    org.opencontainers.image.description="Nodejs container image running on Alpine Linux" \
    org.opencontainers.image.authors="Dominic Taylor <dominic@yobasystems.co.uk>" \
    org.opencontainers.image.vendor="Yoba Systems" \
    org.opencontainers.image.version="current" \
    org.opencontainers.image.url="https://hub.docker.com/r/yobasystems/alpine-nodejs/" \
    org.opencontainers.image.source="https://github.com/yobasystems/alpine-nodejs" \
    org.opencontainers.image.revision=$VCS_REF \
    org.opencontainers.image.created=$BUILD_DATE

ARG NODE_VER=20.8.0
ARG NPM_VER=10

RUN apk -U add curl git make gcc g++ python3 linux-headers paxctl libgcc libstdc++ binutils-gold ca-certificates \
 && cd /tmp \
 && curl --silent --ssl https://nodejs.org/dist/v$NODE_VER/node-v$NODE_VER.tar.gz | tar zxf - \
 && cd node-v$NODE_VER \
 && ./configure --prefix=/usr \
 && make -j4 && make install \
 && paxctl -cm /usr/bin/node \
 && npm install -g npm@$NPM_VER \
 && find /usr/lib/node_modules/npm -name test -o -name .bin -type d \
 | xargs rm -rf \
 && apk del \
    curl \
    git \
    make \
    gcc \
    g++ \
    python \
    linux-headers \
    paxctl \
    grep \
    binutils-gold \
    ca-certificates \
 && rm -rf \
    /tmp/* \
    /var/cache/apk/* \
    /root/.npm \
    /root/.node-gyp \
    /usr/lib/node_modules/npm/man \
    /usr/lib/node_modules/npm/doc \
    /usr/lib/node_modules/npm/html \
    /usr/share/man

CMD ["node", "-v"]
