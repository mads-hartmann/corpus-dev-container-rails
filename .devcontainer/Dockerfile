FROM mcr.microsoft.com/devcontainers/ruby:3.4-bookworm

USER root

RUN apt-get update \
  && apt-get install --no-install-recommends -y libsqlite3-dev libvips sqlite3 \
  && rm -rf /var/lib/apt/lists/*

USER vscode
