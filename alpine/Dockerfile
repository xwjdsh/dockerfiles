FROM alpine
MAINTAINER Wendell Sun <sunwen@kxkr.com>

RUN apk --no-cache add tzdata ca-certificates && update-ca-certificates && ls -al /etc/ssl/
RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
RUN echo "Asia/Shanghai" >  /etc/timezone

CMD ["/bin/sh"]
