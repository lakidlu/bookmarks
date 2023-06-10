FROM python:3.12-rc-alpine3.18

WORKDIR /usr/src/bookmarks

# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# install dependencies
RUN pip install --upgrade pip
COPY ./requirements.txt /usr/src/bookmarks/requirements.txt
RUN pip install -r requirements.txt

# copy project
COPY ./bookmarks /usr/src/bookmarks

