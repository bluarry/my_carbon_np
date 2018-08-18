#FROM debian:9.5
FROM debian:latest 
COPY dock_source/sources.list /etc/apt/sources.list
RUN 	\
  	apt-get update && apt-get install -y wget nginx memcached vim php7.0-fpm php7.0-xml php7.0-mysqlnd php7.0-curl php7.0-gd php7.0-mbstring;
COPY dock_source/start.sh /
RUN chmod +x start.sh
CMD ["bash","/start.sh"]
WORKDIR /var/www/html

