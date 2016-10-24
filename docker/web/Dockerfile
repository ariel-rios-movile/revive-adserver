FROM nginx:latest
MAINTAINER Ariel Gerardo Ríos <ariel.rios@movile.com>

RUN ["apt-get", "update"]
RUN ["apt-get", "install", "-y", "telnet", "wget"]

RUN ["mkdir", "-p", "/movile/adserver"]
RUN ["mkdir", "-p", "/movile-logs/adserver"]

WORKDIR /movile/adserver

COPY ["site.conf", "/etc/nginx/conf.d/default.conf"]
