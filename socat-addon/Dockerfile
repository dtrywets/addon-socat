ARG BUILD_FROM=hassioaddons/base:edge
FROM ${BUILD_FROM}

SHELL ["/bin/bash", "-o", "pipefail", "-c"]
ENV LANG C.UTF-8

# Install socat
RUN apk add --no-cache socat

# Copy s6 overlay services
COPY rootfs/etc /etc

# No CMD: HA will use /init
