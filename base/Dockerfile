FROM ubuntu:trusty

MAINTAINER tom@subledger.com

ENV DOCKER_IMAGE=skulltronix/trusty \
    TERM=xterm-256color

RUN apt-get update -y

RUN apt-get -o Dpkg::Options::="--force-confnew" \
            dist-upgrade -y

RUN apt-get install -y    \
      build-essential     \
      chrpath             \
      cpio                \
      diffstat            \
      gawk                \
      gcc-multilib        \
      git-core            \
      git-email           \
      libaio-dev          \
      libbluetooth-dev    \
      libbrlapi-dev       \
      libbz2-dev          \
      libcap-dev          \
      libcap-ng-dev       \
      libcurl4-gnutls-dev \
      libgtk-3-dev        \
      libibverbs-dev      \
      libjpeg8-dev        \
      liblzo2-dev         \
      libncurses5-dev     \
      libnuma-dev         \
      librbd-dev          \
      librdmacm-dev       \
      libsasl2-dev        \
      libsdl1.2-dev       \
      libseccomp-dev      \
      libsnappy-dev       \
      libssh2-1-dev       \
      libtool             \
      libvde-dev          \
      libvdeplug-dev      \
      libvte-2.90-dev     \
      libxen-dev          \
      python              \
      socat               \
      texinfo             \
      unzip               \
      valgrind            \
      wget                \
      xfslibs-dev         \
      xterm               \
      zip
