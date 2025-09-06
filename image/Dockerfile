FROM alpine:3.16.7
MAINTAINER Chris Dornsife <chris@applariat.com>

RUN apk add --no-cache ca-certificates postfix rsyslog supervisor \
    && /usr/bin/newaliases

COPY . /

EXPOSE 25

ENTRYPOINT [ "/tx-smtp-relay.sh" ]

