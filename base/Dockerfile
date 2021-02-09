FROM ubuntu

ARG USER=bfreire
ARG UID=1000
ARG GID=1000

RUN groupadd -g $GID $USER \
    && useradd -m -u $UID -g $GID $USER \
    && mkdir /workspace \
    && chown $UID:$GID -R /workspace

    && apt update -yqq \
    && apt install -yqq git-flow \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace

USER $USER
