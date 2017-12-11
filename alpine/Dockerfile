FROM alpine
LABEL maintainer="Wendell"

RUN apk --no-cache add tzdata ca-certificates && update-ca-certificates \
			&& cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
			&& echo "Asia/Shanghai" >  /etc/timezone

CMD ["/bin/sh"]
