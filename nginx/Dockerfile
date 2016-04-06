# Nginx, Gunicorn, Django
#
# VERSION               0.0.1

FROM nginx

MAINTAINER Joao Manoel Lins <joaomanoellins@gmail.com>

LABEL Description="This image is used to start a Django Project with Nginx and Gunicorn"

RUN mkdir -p /etc/nginx/sites-available/

WORKDIR /etc/nginx/sites-available/

COPY django .
