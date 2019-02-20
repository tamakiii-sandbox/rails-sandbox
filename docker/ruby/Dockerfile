FROM ruby:2.6.1-alpine

RUN apk add --update build-base linux-headers libxml2-dev libxslt-dev mysql-dev postgresql-dev sqlite-dev nodejs tzdata

COPY ./Gemfile /tmp/
COPY ./Gemfile.lock /tmp/
RUN cd /tmp && bundle install
