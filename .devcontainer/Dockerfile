FROM mcr.microsoft.com/devcontainers/ruby:3.4-bookworm

RUN apt-get update \
    && export DEBIAN_FRONTEND=noninteractive \
    && apt-get install -y --no-install-recommends libvips sqlite3 \
    && rm -rf /var/lib/apt/lists/*
