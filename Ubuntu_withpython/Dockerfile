# Pull base image.
FROM ubuntu:20.04
FROM mcr.microsoft.com/dotnet/core/sdk:2.1.807-bionic
 
LABEL maintainer="Judith Silvina <judith.silvina@xxxxxxxxxx.xxx>"
 
# Install updates to base image
RUN apt-get update \
  && apt-get install -y python2.7

RUN apt-get update \
  && apt-get install -y python3.8 python3-pip python3.8-dev \
  && pip3 install --upgrade pip

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update \
  && apt-get install -y tzdata \
  && dpkg-reconfigure --frontend noninteractive tzdata