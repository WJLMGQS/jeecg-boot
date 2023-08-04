FROM anapsix/alpine-java:8_server-jre_unlimited
LABEL name="wjlmgqs/mtdelog-boot" version="1.0"

MAINTAINER wjlmgqs@sina.com

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

RUN mkdir -p /jeecg-system-cloud

WORKDIR /jeecg-system-cloud

EXPOSE 7001

ADD ./jeecg-system-cloud-start-3.5.2.jar ./

CMD sleep 1;java -Dfile.encoding=utf-8 -Djava.security.egd=file:/dev/./urandom -jar jeecg-system-cloud-start-3.5.2.jar
