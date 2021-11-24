FROM ubuntu:20.04
LABEL maintainer="d.h@s.c"
RUN apt update \
    && apt -y install jq \
    && apt clean

WORKDIR /usr/src/app
COPY prg ./
RUN chmod -R 755 /usr/src/app/prg
RUN ./prg
