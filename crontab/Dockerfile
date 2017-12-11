FROM alpine
LABEL maintainer="Wendell"


RUN echo '*/5 * * * * echo "*/5 * * * *" > crontab.tmp \
  && echo '0 0 * * * echo "0 0 * * *" >> crontab.tmp \
  && echo '0 0 1 * * echo "0 0 1 * *" >> crontab.tmp \
	&& crontab crontab.tmp \
  && rm -rf crontab.tmp

ENTRYPOINT ["/bin/sh", "-c", "/usr/sbin/crond -f -d 0"]
