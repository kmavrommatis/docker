
FROM ubuntu:latest

RUN apt-get update && apt-get install wget

WORKDIR /opt
wget ftp://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/LATEST/ncbi-blast-2.7.1+-x64-linux.tar.gz && \
tar -xvzf ncbi-blast-2.7.1+-x64-linux.tar.gz

WORKDIR /opt/ncbi-blast-2.7.1+/bin
RUN ln -s /opt/ncbi-blast-2.7.1+/bin/blast_formatter /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/blastdb_aliastool /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/blastdbcheck /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/blastdbcmd /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/blastn /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/blastp /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/blastx /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/convert2blastmask /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/deltablast /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/dustmasker /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/legacy_blast.pl /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/makeblastdb /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/makembindex /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/makeprofiledb /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/psiblast /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/rpsblast /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/rpstblastn /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/segmasker /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/tblastn /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/tblastx /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/update_blastdb.pl /usr/local/bin &&\
/opt/ncbi-blast-2.7.1+/bin/windowmasker /usr/local/bin
