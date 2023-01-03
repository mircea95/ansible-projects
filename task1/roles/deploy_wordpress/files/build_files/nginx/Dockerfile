FROM alpine:latest
RUN apk update &&\
    apk upgrade
RUN apk add nginx

ENTRYPOINT ["nginx", "-g", "daemon off;"]