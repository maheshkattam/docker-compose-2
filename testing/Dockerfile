FROM ubuntu:14.04

MAINTAINER giri <veeraraju1993@gmail.com>

RUN apt-get update && apt-get install -y apache2 apache2-threaded-dev && apt-get install -y vim

# Configure localhost in Apache
RUN echo "ServerName localhost" >> /etc/apache2/apache2.conf

WORKDIR /etc/apache2/sites-available/
#ADD  ../server_files/* /etc/apache2/sites-available/
#ADD ../ssl_11222016 /etc/apache2/ssl_11222016
COPY . /madi
#RUN a2enmod ssl
#RUN a2enmod proxy
#RUN a2enmod proxy_connect
#RUN a2enmod proxy_http
#RUN a2enmod proxy_balancer

#RUN a2ensite 0api.conf
#RUN a2ensite 0api_ssl.conf


#Expose Apache
Expose 80
# Define default command
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
