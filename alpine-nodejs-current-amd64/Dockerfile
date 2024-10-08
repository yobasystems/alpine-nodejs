FROM yobasystems/alpine:3.20.2-amd64

ARG BUILD_DATE
ARG VCS_REF

LABEL maintainer="Dominic Taylor <dominic@yoba.systems>" \
    architecture="amd64/x86_64" \
    nodejs-version="current" \
    alpine-version="3.20.2" \
    build="19-Aug-2024" \
    org.opencontainers.image.title="alpine-nodejs" \
    org.opencontainers.image.description="Nodejs container image running on Alpine Linux" \
    org.opencontainers.image.authors="Dominic Taylor <dominic@yoba.systems>" \
    org.opencontainers.image.vendor="Yoba Systems" \
    org.opencontainers.image.version="current" \
    org.opencontainers.image.url="https://hub.docker.com/r/yobasystems/alpine-nodejs/" \
    org.opencontainers.image.source="https://github.com/yobasystems/alpine-nodejs" \
    org.opencontainers.image.base.name="docker.io/yobasystems/alpine:3.20.2" \
    org.opencontainers.image.revision=$VCS_REF \
    org.opencontainers.image.created=$BUILD_DATE

ARG NODE_VER=22.6.0
ARG NPM_VER=10

RUN addgroup -g 1000 node \
 && adduser -u 1000 -G node -s /bin/sh -D node \
 && apk -U add bash curl git make gcc g++ gnupg python3 linux-headers paxctl libgcc libstdc++ binutils-gold ca-certificates ccache xz \
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
    bash \
    curl \
    git \
    make \
    gcc \
    g++ \
    gnupg \
    python3 \
    linux-headers \
    paxctl \
    grep \
    binutils-gold \
    ca-certificates \
    ccache \
    xz \
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
