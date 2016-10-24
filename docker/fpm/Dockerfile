FROM php:5-fpm
MAINTAINER Ariel Gerardo Ríos <ariel.rios@movile.com>

RUN ["apt-get", "update"]
RUN ["apt-get", "install", "-y", "telnet", "wget"]

RUN ["docker-php-ext-install", "mysqli"]
RUN ["sed", "-ri", "s/^www-data:x:33:33:/www-data:x:1000:50:/", "/etc/passwd"]
