FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04

# Install Node.js and npm
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends curl ca-certificates \
    && curl -fsSL https://deb.nodesource.com/setup_lts.x | bash - \
    && apt-get -y install --no-install-recommends nodejs \
    && apt-get clean -y && rm -rf /var/lib/apt/lists/*
