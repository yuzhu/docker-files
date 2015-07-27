FROM java:latest
MAINTAINER David Zhu
# Get Tachyon from github release`.
RUN mkdir -p /opt && \
    cd /opt && \
    wget https://github.com/amplab/tachyon/releases/download/v0.7.0/tachyon-0.7.0-bin.tar.gz && \
    tar -zvxf tachyon-0.7.0-bin.tar.gz && \
    rm tachyon-0.7.0-bin.tar.gz && \
    ln -s tachyon-0.7.0 tachyon && \
    echo Tachyon installed in /opt

ENV PATH $PATH:/opt/tachyon/bin
