FROM ubuntu:xenial
MAINTAINER Andrej Kyselica andrej@kyselica.com
USER root

RUN apt-get update && \
    apt-get install python python-pip  -y && \
    apt-get clean

RUN pip install --upgrade pip && \
    pip install jupyter && \
    pip install bash_kernel && \ 
    python -m bash_kernel.install

USER $NB_USER