FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04

# System libraries required by the application:
# - libvips: image_processing gem (Active Storage variants)
# - libsqlite3-dev / sqlite3: SQLite database adapter and CLI
# - libyaml-dev / build-essential: native gem compilation
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
        build-essential \
        libvips \
        libsqlite3-dev \
        sqlite3 \
        libyaml-dev \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
