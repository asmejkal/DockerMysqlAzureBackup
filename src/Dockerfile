FROM alpine:latest

COPY ./scripts/daily/* /etc/periodic/daily

RUN apk update && \
    apk upgrade && \
    apk add --no-cache mariadb-client && \
	apk add --update npm && \
	npm install -g n azure-cli && \
    chmod a+x /etc/periodic/daily/*

ENTRYPOINT ["crond", "-f", "-d", "8"]
