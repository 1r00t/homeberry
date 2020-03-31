FROM python:3.7-alpine

ENV PYTHONUNBUFFERED=1

WORKDIR /api

COPY ./requirements.txt /api/requirements.txt

RUN pip install -r requirements.txt

COPY . /app

RUN adduser -D api_user
USER api_user
