#
# Dockerfile for nmap + rtsp stream discovery scripts
#

FROM ubuntu:18.04
MAINTAINER Deepak <deepak.muley@gmail.com>

WORKDIR /data

RUN apt update \
  && apt install -y wget \
  && wget http://www.happytimesoft.com/downloads/happytime-onvif-server.tar.gz \
  && tar -xvzf happytime-onvif-server.tar.gz

ENTRYPOINT [ "/bin/sh" ]