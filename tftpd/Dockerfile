FROM alpine:3.5

MAINTAINER community@apstra.com

RUN apk --no-cache add tftp-hpa

EXPOSE 69/udp

RUN adduser -D tftp

ENTRYPOINT ["in.tftpd"]
CMD ["--foreground", "--verbose", "-u", "tftp", "--secure", "/tftpboot"]