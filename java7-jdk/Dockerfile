FROM debian:jessie

ENV MINOR_VERSION 72
ENV BUILD_NUMBER b14

RUN apt-get update && apt-get install -y curl && \
    (curl -skLb "oraclelicense=accept-securebackup-cookie" http://download.oracle.com/otn-pub/java/jdk/7u$MINOR_VERSION-$BUILD_NUMBER/jdk-7u$MINOR_VERSION-linux-x64.tar.gz  | tar xfz -)

ENV JAVA_HOME /jdk1.7.0_$MINOR_VERSION
ENV PATH $PATH:$JAVA_HOME/bin

