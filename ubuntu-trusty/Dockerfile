# ubuntu:trusty
# https://github.com/nmarus/docker-images
# Nicholas Marus <nmarus@gmail.com>

FROM ubuntu:trusty
MAINTAINER Nicholas Marus <nmarus@gmail.com>

# Setup APT
RUN echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections

# Update container
RUN DEBIAN_FRONTEND=noninteractive apt-get -y update && \
    apt-get -y upgrade && \
    apt-get clean
