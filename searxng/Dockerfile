FROM docker.io/searxng/searxng:latest

# Copy static settings that enable JSON format (used by upstream entrypoint)
COPY settings.yml /etc/searxng/settings.yml
ENV SEARXNG_SETTINGS_PATH=/etc/searxng/settings.yml

# SearXNG listens on 8787 internally
ENV GRANIAN_PORT=8787
EXPOSE 8787

# Use the base image's default entrypoint; our settings.yml is referenced via SEARXNG_SETTINGS_PATH

