FROM python:3.8-alpine

MAINTAINER Winston Pacheco Junior "winston(at)atleastonce.cc"

COPY ./requirements.txt /app/requirements.txt
WORKDIR /app
RUN pip install -r requirements.txt
COPY . /app
ENV FLASK_APP app.py
CMD flask run --host=0.0.0.0
