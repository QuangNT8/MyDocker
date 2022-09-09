FROM ubuntu:22.04

RUN apt-get update \
 && apt-get install -y wget \
 && rm -rf /var/lib/apt/lists/*

RUN wget https://go.dev/dl/go1.19.1.linux-arm64.tar.gz

RUN tar -C /usr/local -xzf go1.19.1.linux-arm64.tar.gz

RUN rm go1.19.1.linux-arm64.tar.gz

# Configure Go
ENV PATH=$PATH:/usr/local/go/bin

RUN go version
