FROM alpine
MAINTAINER Wendell Sun <iwendellsun@gmail.com>

WORKDIR /
RUN apk add --no-cache wget
RUN wget https://github.com/shadowsocks/shadowsocks-go/releases/download/1.2.1/shadowsocks-server.tar.gz --no-check-certificate
RUN tar -zxvf shadowsocks-server.tar.gz && chmod +x shadowsocks-server

EXPOSE 3389
ENTRYPOINT ["/shadowsocks-server","-p","3389"]
