FROM ubuntu:22.04

ARG DEBIAN_FRONTEND=noninteractive

RUN apt update
RUN apt upgrade -y

RUN apt-get install -y mp3wrap \
  && rm -rf /var/lib/apt/lists/*

RUN rm -rf /var/lib/apt/lists/*
RUN apt clean

RUN useradd -ms /bin/bash apprunner
USER apprunner
WORKDIR /home/apprunner
