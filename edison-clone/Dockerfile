FROM skulltronix/sklltrnx

MAINTAINER tom@subledger.com

ENV DOCKER_IMAGE=skulltronix/edison-clone \
    TERM=xterm-256color                   \
    YOCTO=iot-devkit-yp-poky-edison-20160606

RUN wget http://iotdk.intel.com/src/3.5/edison/$YOCTO.zip && \
    unzip $YOCTO.zip                                      && \
    rm $YOCTO.zip
