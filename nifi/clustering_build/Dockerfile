FROM apache/nifi:1.14.0

USER root

ADD requirements.txt /tmp/project/

RUN apt-get update && \
    apt-get install -y vim && \
    apt-get install -y python3 python3-pip && \
    pip3 install --no-cache-dir -r /tmp/project/requirements.txt && \
    rm -rf \
    /tmp/* \
    /var/lib/apt/lists/*

