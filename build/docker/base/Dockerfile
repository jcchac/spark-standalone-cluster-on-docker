ARG debian_buster_image_tag=11.0.8-jre-slim
FROM openjdk:${debian_buster_image_tag}

# -- Layer: OS + Python

ARG shared_workspace=/opt/shared_workspace

RUN mkdir -p ${shared_workspace} && \
    apt-get update -y && \
    apt-get install -y curl python3 && \
    ln -s /usr/bin/python3 /usr/bin/python && \
    rm -rf /var/lib/apt/lists/*

ENV SHARED_WORKSPACE=&{shared_workspace}

# -- Runtime

VOLUME ${shared_workspace}
CMD ["bash"]