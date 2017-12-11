FROM alpine
LABEL maintainer="Wendell"

RUN apk add --no-cache wget \
			&& wget https://github.com/xtaci/kcptun/releases/download/v20171201/kcptun-linux-amd64-20171201.tar.gz --no-check-certificate -O kcptun.gz \
			&& tar -zxvf kcptun.gz && rm kcptun.gz server_linux_amd64 && mv client_linux_amd64 kcptun_client

EXPOSE 3389
ENTRYPOINT ["/kcptun_client","-l",":3389"]
