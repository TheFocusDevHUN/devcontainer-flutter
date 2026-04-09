FROM mcr.microsoft.com/devcontainers/base:trixy

ARG FLUTTER_VERSION=3.19.6-stable

RUN apt-get update && apt-get install -y curl xz-utils git unzip

RUN curl -L https://storage.googleapis.com/flutter_infra_release/releases/stable/linux/flutter_linux_${FLUTTER_VERSION}.tar.xz \
    | tar -xJ -C /opt

ENV PATH="/opt/flutter/bin:/opt/flutter/bin/cache/dart-sdk/bin:${PATH}"