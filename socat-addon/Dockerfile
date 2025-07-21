ARG BUILD_FROM=hassioaddons/base:edge
FROM ${BUILD_FROM}

SHELL ["/bin/bash", "-o", "pipefail", "-c"]
ENV LANG C.UTF-8

# Install socat
RUN apk add --no-cache socat

# Copy s6 overlay services (run & finish)
COPY rootfs/etc /etc

# Use the s6-overlay init system as PID 1
ENTRYPOINT ["/init"]
