FROM mcr.microsoft.com/devcontainers/ruby:3.4

# System libraries required by the app's gems:
# - libvips: image_processing gem (Active Storage variants)
# - sqlite3 + libsqlite3-dev: SQLite database used by Active Record
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends libvips sqlite3 libsqlite3-dev \
    && apt-get clean && rm -rf /var/lib/apt/lists/*
