# using the jdk image that we configure before

FROM centos/jdk8:v1

MAINTAINER MOHD_IZHAR mdizhar@gmail.com

RUN mkdir tools

WORKDIR tools

COPY apache* .

RUN tar -xvzf apache* 

RUN mv apache-tomcat-8.5.57 /tomcat


ENV CATALINA_BASE /tomcat
ENV CATALINA_TMPDIR /tomcat/temp
ENV JAVA_JRE /usr/java/jdk1.8.0_171-amd64
COPY sample* /tomcat/webapps

CMD ["/tomcat/bin/catalina.sh", "run"]

EXPOSE 8080
