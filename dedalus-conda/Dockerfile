FROM continuumio/miniconda3

WORKDIR /home/dedalus
RUN wget https://raw.githubusercontent.com/DedalusProject/dedalus_conda/master/install_conda.sh

SHELL ["conda", "run", "-n", "base", "/bin/bash", "-c"]
RUN source /home/dedalus/install_conda.sh

EXPOSE 22
CMD ["/usr/sbin/sshd", "-D"]