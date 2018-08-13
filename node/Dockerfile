# Specify a base image.
FROM debian:stable-slim

# Install build prep tools.
RUN apt-get update && apt-get install -y xz-utils --no-install-recommends
ADD https://nodejs.org/dist/v8.11.3/node-v8.11.3-linux-x64.tar.xz /

# Install node binaries.
RUN tar -xf /node-v8.11.3-linux-x64.tar.xz \
  && rm /node-*.tar.xz \
  && mv /node-* /usr/lib/node \
  && ln -s /usr/lib/node/bin/node /usr/bin \
  && ln -s /usr/lib/node/bin/npm /usr/bin

# Build app.
RUN mkdir -p /srv/node
RUN echo "console.log('hello')" > /srv/node/index.js

# Set working directory.
WORKDIR /srv/node

# Run app.
CMD ["node", "/srv/node/index.js"]
