FROM resin/raspberrypi3-debian:stretch

ENV INITSYSTEM=on

WORKDIR /app

# Update image
SHELL ["/bin/bash", "-c"]

RUN apt-get update && apt-get install -y \
    cmake \
    build-essential \
    curl \
    libcurl4-openssl-dev \
    libssl1.0-dev \
    libffi-dev \
    uuid-dev \
    apt-utils \ 
    python \
    python-pip \
    python-virtualenv \
    python-setuptools \
    python3 \
    python3-pip \
    python3-virtualenv \
    libboost-python-dev \
    pkg-config \
    valgrind 

COPY requirements.txt ./
RUN pip install -r requirements.txt
