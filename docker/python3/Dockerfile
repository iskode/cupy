FROM nvidia/cuda:11.2.2-cudnn8-devel

RUN apt-get update -y && \
    apt-get install -y --no-install-recommends \
    python3-dev \
    python3-pip \
    python3-wheel \
    python3-setuptools && \
    rm -rf /var/lib/apt/lists/* /var/cache/apt/archives/*

RUN pip3 install --no-cache-dir -U install setuptools pip
RUN pip3 install --no-cache-dir  -f https://github.com/cupy/cupy/releases/v10.0.0b2 "cupy-cuda112[all]==10.0.0b2"
