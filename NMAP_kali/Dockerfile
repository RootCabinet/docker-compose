# Use the latest official Kali Linux base image
FROM kalilinux/kali-rolling:latest

# Prevent dpkg/apt from asking questions during installation
ENV DEBIAN_FRONTEND=noninteractive

# Update package list and install necessary packages:
# nmap for network scanning
# procps for utilities like ps (useful for debugging)
# net-tools for utilities like ifconfig, route
# iputils-ping for ping
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    openssh-server \
    nmap \
    procps \
    net-tools \
    iputils-ping && \
    apt-get clean autoclean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
