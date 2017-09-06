FROM golang:1.9.0-alpine3.6 

RUN apk update --no-cache \
    && apk add --no-cache --virtual .build-deps \
        git openssh \
    && go get github.com/labstack/echo \
    && apk del -f .build-deps