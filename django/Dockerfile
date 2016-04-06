# Nginx, Gunicorn, Django
#
# VERSION               0.0.1

FROM django:1.9.5

MAINTAINER Joao Manoel Lins <joaomanoellins@gmail.com>

LABEL Description="This image is used to start a Django Project with Nginx and Gunicorn"

RUN mkdir -p /home/django

WORKDIR /home/django

COPY ./app/helloworld .

EXPOSE 9000

CMD ["python", "manage.py", "runserver", "0.0.0.0:9000"]
