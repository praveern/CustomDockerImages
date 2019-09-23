# Base docker file to act as dummy base image for customized usages

FROM ubuntu:latest
MAINTAINER praveern "pnarwelkar@gmail.com"

RUN apt-get update \
  && apt-get install -y python3-pip python3==3.6.1 \
  && cd /usr/local/bin \
  && ln -s /usr/bin/python3 python \
  && pip3 install --upgrade --no-cache-dir pip

ENTRYPOINT ["python3"]