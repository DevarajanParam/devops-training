# This is a sample file
FROM centos:latest
MAINTAINER parmeshd@rediffmail.com
RUN yum -y install httpd
ADD code /var/www/html
EXPOSE 80
ENV applb=test
CMD ["apachectl","-D","FOREGROUND"]
