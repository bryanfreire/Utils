FROM ubuntu AS exercism

ARG EXERCISM_VERSION=3.0.13
ARG EXERCISM_FILE=exercism-${EXERCISM_VERSION}-linux-x86_64.tar.gz
ARG EXERCISM_BASE_URL=https://github.com/exercism/cli/releases/download
ARG EXERCISM_URL=${EXERCISM_BASE_URL}/v${EXERCISM_VERSION}/${EXERCISM_FILE}

RUN apt update -yqq \
    && apt install -yqq wget \
    && wget $EXERCISM_URL \
    && tar zxf $EXERCISM_FILE \
    && mv exercism /bin/
