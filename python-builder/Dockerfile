ARG BASE=ubuntu:22.04
FROM ${BASE}

RUN apt-get update && apt-get install -y --no-install-recommends \
  build-essential \
  ca-certificates \
  clang-15 \
  git \
  libbz2-dev \
  libffi-dev \
  liblzma-dev \
  libreadline-dev \
  libssl-dev \
  libsqlite3-dev \
  sudo \
  wget \
  zlib1g-dev \
  && rm -rf /var/lib/apt/lists/*

RUN useradd -rm -d /home/ubuntu -s /bin/bash ubuntu
RUN echo "ubuntu ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers
USER ubuntu
ENV HOME="/home/ubuntu"
ENV PATH="/usr/lib/llvm-15/bin:$PATH"
ENV CC="clang"
ENV CXX="clang++"