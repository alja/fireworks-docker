FROM ubuntu:20.04
MAINTAINER aljamrak
RUN apt update
RUN apt-get update
RUN apt-get install -y libgl1-mesa-glx
RUN apt-get install -y libglu1
RUN apt-get install -y vim
RUN apt-get install -y libfreetype6
RUN apt-get install -y grep
RUN apt-get install -y libice6
RUN apt-get install -y libsm6
RUN apt-get install -y libxpm4
RUN apt-get install -y libgssapi-krb5-2
RUN apt-get install -y libncurses5
RUN apt-get install -y mesa-utils
RUN apt-get install -y libxft2
RUN apt-get install -y iputils-ping
RUN apt-get install -y libc6-dev
RUN apt-get install -y libopengl-dev
RUN apt-get install -y libgl-dev
ADD cmsShow-11.1.2.tar.gz /
WORKDIR "/cmsShow-11.1.2"
