# Nginx, Gunicorn, Django
#
# VERSION               0.0.1

FROM python:3.4

MAINTAINER Joao Manoel Lins <joaomanoellins@gmail.com>

LABEL Description="This image is used to start a Django Project with Nginx and Gunicorn"

ENV PYTHONUNBUFFERED 1

RUN easy_install pip 

RUN pip install gunicorn

WORKDIR /etc/init/

COPY gunicorn.conf .

WORKDIR /etc/gunicorn.d/

COPY gunicorn.py .

CMD ["service" "nginx" "restart"]

CMD ["service", "gunicorn", "start"]
