FROM resin/rpi-raspbian:wheezy
MAINTAINER t.hixson08@gmail.com

RUN apt-get update \
    && apt-get install -y wget \
    && wget http://nodejs.org/dist/v0.12.7/node-v0.12.7.tar.gz \
    && tar -xzf node-v0.12.7.tar.gz \
    && apt-get install -y gcc \
    && apt-get install -y make\ 
    && apt-get install -y g++ \
    && apt-get install -y python \
    && cd node-v0.12.7 \
    && ./configure \
    && make \
    && make install

WORKDIR /home/default