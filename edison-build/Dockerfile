FROM skulltronix/edison-clone

MAINTAINER tom@subledger.com

ENV DOCKER_IMAGE=skulltronix/edison-build \
    TERM=xterm-256color

WORKDIR /home/sklltrnx/$YOCTO/poky

RUN source ./oe-init-build-env ../build_edison/          && \
    bitbake edison-image u-boot                          && \
    ../poky/meta-intel-edison/utils/flash/postBuild.sh . && \
    zip -r toFlash.zip toFlash

WORKDIR /home/sklltrnx

# nasm
# yasm
# pcre
# glib
# orc

# mad
# mpg123-dev
# libav
# gstreamer
# gst-plugins-base
# gst-plugins-good
# gst-plugins-ugly
# gst-libav

# partially removable
# # ${TOPDIR}/../poky/meta-intel-iot-middleware/recipes-connectivity
# ${TOPDIR}/../poky/meta-intel-iot-devkit/recipes-connectivity/ofono

# modify due to removables
# ${TOPDIR}/../poky/meta-intel-iot-devkit/recipes-core/initscripts
# ${TOPDIR}/../poky/meta-intel-iot-devkit/recipes-core/packagegroups/meta-intel-iot-extra
# ${TOPDIR}/../poky/meta-intel-iot-devkit/recipes-core/packagegroups/meta-intel-iot # remove numpy ruby apache2

# completely removable
# ${TOPDIR}/../poky/meta-intel-edison/meta-intel-arduino \
# ${TOPDIR}/../poky/meta-java \
# ${TOPDIR}/../poky/meta-openembedded/meta-python \
# ${TOPDIR}/../poky/meta-openembedded/meta-ruby \
# ${TOPDIR}/../poky/meta-openembedded/meta-webserver \
