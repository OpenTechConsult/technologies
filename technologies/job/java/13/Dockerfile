FROM openjdk:13.0-jdk-slim-buster

COPY entrypoint /entrypoint
RUN chmod 755 /entrypoint

ENV HADOOP_CONF_DIR=/etc/hadoop/conf

#UPDATE SECURITY PACKAGE BEGIN
RUN apt-get update && apt-get upgrade -y
#UPDATE SECURITY PACKAGE END

WORKDIR /sandbox

ENTRYPOINT  ["bash","/entrypoint"]