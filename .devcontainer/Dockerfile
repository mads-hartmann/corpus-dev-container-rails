FROM mcr.microsoft.com/devcontainers/ruby:3.4-bookworm

RUN apt-get update \
    && apt-get install --no-install-recommends -y libvips sqlite3 \
    && rm -rf /var/lib/apt/lists/*
