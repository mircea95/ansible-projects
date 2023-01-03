FROM alpine:latest

# WORKDIR /app

RUN apk add --update mysql mysql-client && rm -f /var/cache/apk/*

COPY startup.sh .
# COPY my.cnf /etc/mysql/my.cnf
RUN chmod +x startup.sh
RUN dos2unix startup.sh
CMD ["./startup.sh"]
