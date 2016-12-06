FROM alpine
MAINTAINER Wendell Sun <iwendellsun@gmail.com>
WORKDIR /
ENV MODE=fast2
RUN apk add --no-cache wget
RUN wget https://github.com/xtaci/kcptun/releases/download/v20161202/kcptun-linux-amd64-20161202.tar.gz --no-check-certificate -O kcptun.gz
RUN tar -zxvf kcptun.gz && rm kcptun.gz client_linux_amd64 && mv server_linux_amd64 kcptun
EXPOSE 3400
ENTRYPOINT ["/bin/sh", "-c", "/kcptun -t $T -l ':3400' --mode $MODE"]
