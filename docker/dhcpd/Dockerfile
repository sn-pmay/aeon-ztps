FROM alpine:3.5

MAINTAINER community@apstra.com

RUN apk --no-cache add dhcp

EXPOSE 67/udp 67/tcp

RUN ["touch", "/var/lib/dhcp/dhcpd.leases"]

ENTRYPOINT ["dhcpd"]
CMD ["--no-pid", "-4", "-f", "-d"]