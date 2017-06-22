FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y \
    nmap \
    tor \
    wget \
    proxychains \
    python-openssl \
    python-twisted

RUN wget http://downloads.sourceforge.net/project/dnmap/dnmap_v0.6.tgz
RUN tar -xvzf dnmap_v0.6.tgz
ENV NAME=undefined

WORKDIR dnmap_v0.6

CMD echo "start client"; python dnmap_client.py -s dnmap-server -a $NAME
