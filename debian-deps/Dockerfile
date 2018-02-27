FROM dedalusproject/debian-itest
USER root
RUN apt-get -y update && apt-get install -y \
    bc \
    libatlas-base-dev \
    libatlas3-base \
    libssl-dev \
    build-essential \
    libncurses5 \
    libncurses5-dev \
    zip \
    uuid-dev \
    libfreetype6-dev \
    libhdf5-dev \
    libopenmpi-dev \
    openmpi-bin \
    tk-dev \
    mercurial \
    libsqlite3-dev \
    gfortran \
    openssh-server \
    pkg-config

RUN mkdir /var/run/sshd
USER dedalus

CMD /bin/bash