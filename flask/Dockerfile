# FROM ubuntu:18.04
FROM python:3

RUN apt-get -y update
RUN apt-get upgrade

RUN mkdir /app
ADD . /app

WORKDIR /app

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

CMD ["uwsgi","uwsgi.ini"]