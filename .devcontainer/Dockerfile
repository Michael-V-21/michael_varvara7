# Use the default Linux Universal Image
FROM mcr.microsoft.com/devcontainers/universal:2-linux

# Install Node.js (required for Vue.js)
RUN apt-get update && apt-get install -y \
    curl && \
    curl -fsSL https://deb.nodesource.com/setup_18.x | bash - && \
    apt-get install -y nodejs && \
    npm install -g @vue/cli

# Install Python and Flask
RUN apt-get install -y python3 python3-pip && \
    pip install flask

# Set the working directory
WORKDIR /workspace
