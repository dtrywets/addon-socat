ARG BUILD_FROM=ghcr.io/home-assistant/${BUILD_ARCH}-base:latest
FROM ${BUILD_FROM}


ENV LANG C.UTF-8

RUN apk add --no-cache socat

COPY rootfs/etc /etc

# Kein ENTRYPOINT, kein SHELL, kein CMD!
