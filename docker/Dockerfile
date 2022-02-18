
# Set the base image
FROM debian:latest


RUN apt update && apt install -y apache2 libapache2-mod-wsgi build-essential python python-dev python-pip \
 && apt-get clean \
 && apt-get autoremove \
 && rm -rf /var/lib/apt/lists/*

EXPOSE 80

WORKDIR /var/www/flask

CMD  /usr/sbin/apache2ctl -D FOREGROUND