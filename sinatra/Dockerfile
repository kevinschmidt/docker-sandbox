FROM ubuntu:14.04
MAINTAINER Kevin Schmidt "kevin@kevinschmidt.biz"
ENV REFRESHED_AT 2014-09-01
RUN apt-get update
RUN apt-get -y install ruby ruby-dev build-essential redis-tools
RUN gem install --no-rdoc --no-ri sinatra json redis
RUN mkdir -p /opt/webapp
EXPOSE 4567
CMD [ "/opt/webapp/bin/webapp" ]
