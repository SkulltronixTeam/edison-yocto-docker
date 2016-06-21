FROM skulltronix/base

ENV DOCKER_IMAGE=skulltronix/sklltrnx

# Create sklltrnx user, remove default dot files
RUN adduser --disabled-password                            \
            --gecos "info@skulltronix.com"                 \
            sklltrnx                                    && \
    chown root:root /home/sklltrnx/.bashrc              && \
    chown root:root /home/sklltrnx/.bash_logout         && \
    rm /home/sklltrnx/.profile                          && \
    mv /home/sklltrnx/.bashrc /home/sklltrnx/.bashrc.orig

# dotfiles
COPY .bash_profile        /home/sklltrnx/
COPY .bashrc              /home/sklltrnx/
COPY .git-completion.bash /home/sklltrnx/
COPY .git-prompt.bash     /home/sklltrnx/

# use dotfiles for root
RUN rm /root/.profile                      && \
    mv /root/.bashrc /root/.bashrc.orig    && \
    cp /home/sklltrnx/.bashrc /root/.bashrc

# Say goodbye to sh (dash) forever
RUN rm /bin/sh           && \
    ln /bin/bash /bin/sh

WORKDIR /home/sklltrnx
USER    sklltrnx
