

RUN apt-get update && \
apt-get install build-essential git wget unzip

WORKDIR /opt
RUN wget http://github.com/jenniferlu717/Bracken/archive/master.zip &&\
 unzip master.zip
RUN wget http://ccb.jhu.edu/software/kraken/dl/kraken-1.0.tgz && \
 tar -xvzf kraken-1.0.tgz
RUN  wget http://www.cbcb.umd.edu/software/jellyfish/jellyfish-1.1.11.tar.gz &&\
 tar -xvzf jellyfish-1.1.11.tar.gz
WORKDIR /opt/jellyfish-1.1.11
RUN ./configure &&   make && make install

WORKDIR /opt/kraken-1.0
RUN ./install_kraken.sh /opt/kraken-1.0
RUN ln -s /opt/kraken-1.0/kraken /usr/local/bin/ &&\
 ln -s  /opt/kraken-1.0/kraken-build /usr/local/bin/ &&\
 ln -s  /opt/kraken-1.0/kraken-filter /usr/local/bin/ &&\
 ln -s  /opt/kraken-1.0/kraken-mpa-report /usr/local/bin/ &&\
 ln -s  /opt/kraken-1.0/kraken-report /usr/local/bin/ &&\
 ln -s  /opt/kraken-1.0/kraken-translate /usr/local/bin/ 
 
 
