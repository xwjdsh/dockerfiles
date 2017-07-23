FROM alpine
MAINTAINER Wendell Sun <iwendellsun@gmail.com>

WORKDIR /
RUN apk add --no-cache wget gzip
RUN wget https://github.com/shadowsocks/shadowsocks-go/releases/download/1.1.5/shadowsocks-local-linux64-1.1.5.gz --no-check-certificate
RUN gzip -d shadowsocks-local-linux64-1.1.5.gz && chmod +x shadowsocks-local-linux64-1.1.5

EXPOSE 1030
ENTRYPOINT ["/shadowsocks-local-linux64-1.1.5","-l","1030"]
