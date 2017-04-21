FROM debian:latest

RUN apt-get -y update && apt-get install -y wget sudo

RUN useradd -ms /bin/bash dedalus && echo "dedalus:dedalus" | chpasswd && adduser dedalus sudo

USER dedalus
CMD /bin/bash