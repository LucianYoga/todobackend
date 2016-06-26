FROM lucianyoga01/todobackend-base:latest
MAINTAINER Lucian Yogarajah <lucian_y@yahoo.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse
