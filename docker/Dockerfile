FROM python:3.7

LABEL Description="Framework for multiagent systems development in Python. This dockerfile builds a pade production environment."

ENV  FLASK_ENV=production 
ENV  FLASK_DEBUG=0

RUN apt-get update && apt-get install -y python3-pip python-dev build-essential

COPY ./docker/requirements.txt /app/requirements.txt
WORKDIR /app
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

EXPOSE 5000/tcp

CMD sleep infinity
