# Base image
FROM centos:latest

# Author

MAINTAINER MohdIzhar mdizhar@gmial.com

RUN yum update -y && yum install httpd -y

# ADD instruction

ADD https://raw.githubusercontent.com/dugarvineet211/taskpage/master/index.html /var/www/html/


# granting permission for others
RUN chmod 777 /var/www/html/index.html

EXPOSE 80

ENTRYPOINT apachectl "-DFOREGROUND"
