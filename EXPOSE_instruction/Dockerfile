# Base image
FROM centos:latest

# Author

MAINTAINER MohdIzhar mdizhar@gmial.com

# adding user

RUN useradd -ms /bin/bash user

RUN yum update -y && yum install httpd -y && echo "MY DOCKERFILE BUILD WEBSERVER" >/var/www/html/index.html

EXPOSE 80
ENTRYPOINT apachectl "-DFOREGROUND"


