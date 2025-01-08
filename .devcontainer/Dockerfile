FROM ubuntu:22.04

# Install common utilities
RUN apt-get update && apt-get install -y \
    sudo \
    curl \
    vim \
    openssh-server \
    nginx

# Add a default user (vscode)
RUN useradd -ms /bin/bash vscode \
    && echo "vscode ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers.d/vscode
