FROM debian:stable
MAINTAINER govindarajanv <govindarajanv@gmail.com>

RUN apt-get update && apt-get upgrade -y && apt-get install -y apache2 telnet elinks openssh-server

ENV MYVALUE my-value

EXPOSE 80

CMD ["/usr/sbin/apache2ctl","-D","FOREGROUND"]
