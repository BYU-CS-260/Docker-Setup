FROM ubuntu
ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update
RUN apt-get install -y vim curl 
RUN apt-get install -y apache2 apache2-utils
RUN apt-get -y install python3 libapache2-mod-wsgi-py3 
RUN ln /usr/bin/python3 /usr/bin/python 
RUN apt-get -y install python3-pip 
RUN pip install --upgrade pip 

WORKDIR /var/www/html 

EXPOSE 80 3500 
CMD ["apache2ctl", "-D", "FOREGROUND"]