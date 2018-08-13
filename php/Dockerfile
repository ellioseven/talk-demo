# Specify a base image.
FROM debian:stable-slim

# Install php via package manager.
RUN apt-get update && apt-get install -y --no-install-recommends php

# Build app.
RUN mkdir -p /srv/php
RUN echo "<?php echo 'hello\n';" > /srv/php/index.php

# Run app.
CMD ["php", "/srv/php/index.php"]
