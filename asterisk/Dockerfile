FROM ubuntu:22.10
MAINTAINER Iñaki Cívico "icivico@gmail.com"
RUN apt-get update; apt-get -y install asterisk
ENTRYPOINT ["/usr/sbin/asterisk","-f"]
