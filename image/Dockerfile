FROM alpine:3.19.4
MAINTAINER Chris Dornsife <chris@applariat.com>

RUN apk add --no-cache ca-certificates postfix rsyslog supervisor \
    && /usr/bin/newaliases

COPY . /

EXPOSE 25

ENTRYPOINT [ "/tx-smtp-relay.sh" ]

