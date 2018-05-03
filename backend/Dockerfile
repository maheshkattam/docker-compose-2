FROM ubuntu:14.04

MAINTAINER giri <veeraraju1993@gmail.com>

RUN apt-get update && \
    apt-get -y install openjdk-7-jdk 
     
ADD ./apache-tomcat-7.0.23/ /opt/apache-tomcat-7.0.23

ENV JAVA_HOME="/usr/lib/jvm/java-7-openjdk-amd64"

#COPY . /madi
#Expose 80
# Define default command

 
