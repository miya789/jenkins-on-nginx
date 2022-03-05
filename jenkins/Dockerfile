FROM jenkins/jenkins:lts
USER root
RUN apt-get update \
    && apt-get install -y --no-install-recommends net-tools nano procps \
    && apt-get -y clean \
    && rm -rf /var/lib/apt/lists/*
USER jenkins
