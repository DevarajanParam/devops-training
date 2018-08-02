# This is a the file to install ubuntu and other apps
FROM ubuntu:latest
MAINTAINER parmeshd@rediffmail.com
RUN apt-get -y update
ENV TZ=Asia/Kolkata
RUN apt-get -y install tzdata
ADD config /opt
RUN apt-get -y install `cat /opt/packages`
ADD code /var/www/html
EXPOSE 80
CMD ["nginx","-g","daemon off;"]
