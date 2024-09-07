# Use the latest Ubuntu as the base image
FROM ubuntu:latest as base

# Set environment variables to prevent prompts during installations
ENV DEBIAN_FRONTEND=noninteractive

# Update the package list and install essential tools and dependencies
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    build-essential \
    git \
    curl \
    wget \
    ca-certificates \
    software-properties-common \
    python3 \
    python3-pip \
    python3-venv \
    python3-dev \
    python3-setuptools \
    python3-wheel \
    libssl-dev \
    libffi-dev \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# Just create a new image from the base image
FROM base as runner

# Set the working directory
RUN mkdir /workspace
WORKDIR /workspace

# Set the default command to open an interactive shell
CMD ["/bin/bash"]
