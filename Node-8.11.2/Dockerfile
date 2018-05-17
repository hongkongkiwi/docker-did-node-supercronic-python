FROM hongkongkiwi/alpine-node-docker-supercronic:node-8.11.2

MAINTAINER Andy Savage <andy@savage.hk>

LABEL org.label-schema.name="docker-node-docker-supercronic-python" \
      org.label-schema.description="Useful base docker image which includes a base system with Node.js, Docker, Supercronic & Python" \
      org.label-schema.vcs-url="https://github.com/hongkongkiwi/docker-alpine-node-supercronic" \
      org.label-schema.license="MIT"

RUN echo "Installing Packages" \
 && apk add --no-cache \
        python3 \
        python3-dev \
        python \
      	python-dev \
        py2-pip \
 && echo "Upgrading Pip" \
 && pip3 install -q --no-cache-dir --upgrade pip \
 && pip2 install -q --no-cache-dir --upgrade pip \
 && echo "Cleaning Up" \
 && rm -rf ~/.cache/pip \
 && rm -rf /var/cache/apk/*
