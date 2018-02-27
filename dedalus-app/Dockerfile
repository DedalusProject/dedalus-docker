FROM dedalusproject/debian-deps

WORKDIR /home/dedalus
RUN wget https://bitbucket.org/dedalus-project/dedalus/raw/tip/docs/install.sh && bash install.sh -y
RUN mkdir -p /home/dedalus/.config/matplotlib
RUN echo "backend : Agg" >> /home/dedalus/.config/matplotlib/matplotlibrc

VOLUME /output
WORKDIR /output

ENV LD_LIBRARY_PATH /home/dedalus/dedalus/lib:$LD_LIBRARY_PATH
ENV PATH /home/dedalus/dedalus/bin:$PATH
ENV PYTHONPATH /home/dedalus/dedalus/lib/python3.5/site-packages:/home/dedalus/dedalus/src/dedalus

EXPOSE 22
CMD ["/usr/sbin/sshd", "-D"]