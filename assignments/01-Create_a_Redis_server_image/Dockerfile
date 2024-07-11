FROM ubuntu:latest

RUN apt update && \
    apt install -y redis-server

COPY ./redis.conf /etc/redis/

EXPOSE 6380/tcp

USER redis

LABEL MAINTAINER="Giordano Bruno Michela"

ENTRYPOINT [ "redis-server",  "/etc/redis/redis.conf" ]