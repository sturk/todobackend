FROM sturk/todobackend-base:latest
MAINTAINER Serdar Turk  <turkserdar@gmail.com>

# copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse