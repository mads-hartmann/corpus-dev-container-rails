FROM mcr.microsoft.com/devcontainers/ruby:3.4-bookworm

RUN sudo apt-get update \
  && sudo apt-get install --no-install-recommends -y libvips sqlite3 \
  && sudo rm -rf /var/lib/apt/lists/*
