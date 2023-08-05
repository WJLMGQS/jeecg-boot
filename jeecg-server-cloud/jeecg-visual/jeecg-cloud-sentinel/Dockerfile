FROM anapsix/alpine-java:8_server-jre_unlimited
LABEL name="wjlmgqs/mtdelog-sentinel" version="1.0"
MAINTAINER wjlmgqs@sina.com

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

RUN mkdir -p /jeecg-cloud-sentinel

WORKDIR /jeecg-cloud-sentinel

EXPOSE 9000

ADD ./jeecg-cloud-sentinel-3.5.2.jar ./

CMD sleep 5;java -Dfile.encoding=utf-8 -Djava.security.egd=file:/dev/./urandom -jar jeecg-cloud-sentinel-3.5.2.jar
