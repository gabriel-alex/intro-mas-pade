FROM python:3.7

MAINTAINER Pade Development <lucassmelo@dee.ufc.br>

LABEL Description="Framework for multiagent systems development in Python. This dockerfile builds a pade development environment."

ENV  FLASK_ENV=production 
ENV  FLASK_DEBUG=0

RUN apt-get update && apt-get install -y python3-pip python-dev build-essential

COPY ./ /app
WORKDIR /app
RUN pip install --upgrade pip
RUN python setup.py install

EXPOSE 5000/tcp

CMD sleep infinity
