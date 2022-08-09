FROM centos:latest
MAINTAINER Miguel Garza <mgarzago@redhat.com>
ENV JAVA_HOME /usr/lib/jvm/java
RUN cd /etc/yum.repos.d/ && sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-* && \ 
    sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-* && \
    yum -y update && yum -y install unzip tar && \
    yum install -y java-11-openjdk-devel
