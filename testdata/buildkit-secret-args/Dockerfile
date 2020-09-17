# syntax = docker/dockerfile:experimental
FROM busybox
COPY . .
RUN --mount=type=secret,id=secret0,target=/etc/secret/0 cmp /etc/secret/0 secret0
RUN --mount=type=secret,id=secret1,target=/etc/secret/1 cmp /etc/secret/1 secret1
