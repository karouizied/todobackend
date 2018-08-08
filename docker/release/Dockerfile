FROM dockerzied/todobackend-base:latest
MAINTAINER zied karoui <ziedkarouifb@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse