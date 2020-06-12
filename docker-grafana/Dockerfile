FROM netsarang/centos-7

WORKDIR /root

RUN yum update -y
RUN yum install wget -y

RUN wget https://grafanarel.s3.amazonaws.com/builds/grafana-4.1.2-1486989747.linux-x64.tar.gz
RUN tar -xvf grafana-4.1.2-1486989747.linux-x64.tar.gz
RUN rm -f grafana-4.1.2-1486989747.linux-x64.tar.gz

RUN ln -s grafana-4.1.2-1486989747/ grafana
WORKDIR /root/grafana

EXPOSE 3000
