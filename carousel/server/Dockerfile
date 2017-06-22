FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y \
    wget \
    python-openssl \
    python-twisted

RUN wget http://downloads.sourceforge.net/project/dnmap/dnmap_v0.6.tgz
RUN tar -xvzf dnmap_v0.6.tgz
COPY scan.txt dnmap_v0.6

WORKDIR dnmap_v0.6

CMD echo "start server"; python dnmap_server.py -f scan.txt
