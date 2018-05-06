FROM ubuntu:18.04

MAINTAINER BaseBoxOrg <baseboxorg@outlook.com>

RUN apt-get update \
    && DEBIAN_FRONTEND=noninteractive apt-get install -qq --no-install-recommends -y \
    ca-certificates \
    curl \
    && curl https://repogen.simplylinux.ch/txt/bionic/sources_0160feac1dac4f0e8cebd357a27fe236decf035b.txt | tee /etc/apt/sources.list \
    && apt-get update \
    && apt-get remove -y \
    ca-certificates \
    curl \
    && apt-get autoremove -y
