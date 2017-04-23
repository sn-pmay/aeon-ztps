FROM alpine:3.5

MAINTAINER community@apstra.com

RUN apk --no-cache add rsyslog

EXPOSE 514/tcp

ENTRYPOINT ["rsyslogd"]