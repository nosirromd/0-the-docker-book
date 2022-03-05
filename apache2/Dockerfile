FROM unbuntu 14.04
LABEL Maintainer "dc morrison"
LABEL DockerHandle "nosirromd@gmail"
RUN apt-get update
RUN apt_get install -y apache2
ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2
ONBUILD ADD . /var/www/
EXPOSE 80
ENTRYPOINT ["/usr/sbin/apache2"]
CMD ["-D", "FOREGROUND"]