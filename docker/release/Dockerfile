FROM nicolasmartin58/todobackend-base:latest
MAINTAINER nicolasmartin58 <nicolasmartin58@gmail.com>

#  Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse
