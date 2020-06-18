FROM centos:centos7

RUN yum update -y

ADD helpers/darch-extract /darch-extract
ADD helpers/darch-prepare /darch-prepare
ADD helpers/darch-runrecipe /darch-runrecipe
ADD helpers/darch-teardown /darch-teardown


RUN yum install -y wget containerd
RUN wget https://github.com/godarch/darch/releases/download/v0.28.0/darch-amd64.tar.gz
RUN tar -xvf darch-amd64.tar.gz -C /

