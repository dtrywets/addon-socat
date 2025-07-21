ARG BUILD_FROM=ghcr.io/home-assistant/${BUILD_ARCH}-base:latest
FROM ${BUILD_FROM}

SHELL ["/bin/bash", "-o", "pipefail", "-c"]
ENV LANG C.UTF-8

# Install socat + jq
RUN apk add --no-cache socat
RUN apk add --no-cache jq

# Copy s6 overlay services (run & finish)
COPY rootfs/etc /etc
