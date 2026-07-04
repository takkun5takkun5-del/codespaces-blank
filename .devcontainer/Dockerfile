FROM mcr.microsoft.com/devcontainers/universal:2

USER root
RUN apt-get update && apt-get install -y chromium netsurf-gtk && apt-get clean && rm -rf /var/lib/apt/lists/*

USER codespace