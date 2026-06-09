FROM mcr.microsoft.com/devcontainers/ruby:3.4

# libvips is required by the image_processing gem (Active Storage variants).
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends libvips \
    && apt-get clean && rm -rf /var/lib/apt/lists/*
