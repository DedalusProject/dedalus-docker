FROM ubuntu:16.04

RUN apt-get -y update && apt-get install -y \
    lsb-release \
    sudo \      
    wget
    
RUN useradd -ms /bin/bash dedalus && echo "dedalus:dedalus" | chpasswd && adduser dedalus sudo

USER dedalus
CMD /bin/bash