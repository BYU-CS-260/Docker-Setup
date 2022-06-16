FROM mongo
ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update
RUN apt-get install -y vim curl 
RUN apt-get install -y nodejs
RUN apt-get install -y npm
RUN npm install -g http-server
WORKDIR /var/www/html 
EXPOSE 8080
CMD ["http-server"]
