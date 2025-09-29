# task0/Dockerfile
FROM ubuntu:latest

# Prevent interactive tzdata prompts
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update \
 && apt-get upgrade -y \
 && apt-get clean \
 && rm -rf /var/lib/apt/lists/*

# When the container starts, print Hello, World! and exit
CMD ["/bin/sh", "-c", "echo 'Hello, World!'"]
