FROM mcr.microsoft.com/devcontainers/ruby:1-3.4-bookworm

USER root

RUN rm -f /etc/apt/sources.list.d/yarn.list \
  && apt-get update \
  && apt-get install --no-install-recommends -y libvips sqlite3 \
  && rm -rf /var/lib/apt/lists/*

USER vscode
