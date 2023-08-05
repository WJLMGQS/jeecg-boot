FROM anapsix/alpine-java:8_server-jre_unlimited
LABEL name="wjlmgqs/mtdelog-gateway" version="1.0"
MAINTAINER wjlmgqs@sina.com

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

RUN mkdir -p /jeecg-cloud-gateway

WORKDIR /jeecg-cloud-gateway

EXPOSE 9999

ADD ./jeecg-cloud-gateway-3.5.3.jar ./

CMD sleep 1;java -Dfile.encoding=utf-8 -Djava.security.egd=file:/dev/./urandom -jar jeecg-cloud-gateway-3.5.3.jar