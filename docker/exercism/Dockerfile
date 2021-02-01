FROM ubuntu AS exercism

ENV EXERCISM_VERSION 3.0.13
EVN EXERCISM_FILE exercism-${EXERCISM_VERSION}-linux-x86_64.tar.gz
ENV EXERCISM_URL https://github.com/exercism/cli/releases/download/v${EXERCISM_VERSION}/

RUN wget $EXERCISM_URL \
    && tar zxf $EXERCISM_FILE
    && mv exercism /bin/
