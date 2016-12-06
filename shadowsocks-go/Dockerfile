FROM alpine
MAINTAINER Wendell Sun <iwendellsun@gmail.com>
ENV M="aes-256-cfb" T="60"
WORKDIR /
RUN apk add --no-cache wget gzip
RUN wget https://github.com/shadowsocks/shadowsocks-go/releases/download/1.1.5/shadowsocks-server-linux64-1.1.5.gz --no-check-certificate -O ss.gz
RUN gzip -d ss.gz && chmod +x ss
EXPOSE 3389
ENTRYPOINT ["/bin/sh", "-c", "/ss -m $M -t $T -k $K -p 3389"]
