FROM mcr.microsoft.com/devcontainers/python:0-3.10

# Install system dependencies for buildozer and Android
env DEBIAN_FRONTEND=noninteractive
RUN apt-get update && \
    apt-get install -y \
    openjdk-17-jdk \
    python3.10-dev \
    python3.10-venv \
    python3-pip \
    git \
    zip \
    unzip \
    wget \
    libffi-dev \
    libssl-dev \
    libsqlite3-dev \
    zlib1g-dev \
    libncurses5-dev \
    libncursesw5-dev \
    libreadline-dev \
    libgdbm-dev \
    libbz2-dev \
    liblzma-dev \
    libxml2-dev \
    libxslt1-dev \
    libjpeg-dev \
    libfreetype6-dev \
    && apt-get clean

# Set python3.10 as default
RUN update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.10 1
