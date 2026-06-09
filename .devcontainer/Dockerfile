FROM mcr.microsoft.com/devcontainers/ruby:3.4-bookworm

# libvips is required by the image_processing gem; sqlite3 is the application database.
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends libvips sqlite3 \
    && rm -rf /var/lib/apt/lists/*
