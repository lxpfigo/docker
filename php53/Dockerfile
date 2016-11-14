FROM alari/php-fpm-53
ADD php.ini    /etc/php5/fpm/php.ini
ADD ZendGuardLoader.so /usr/local/ext/ZendGuardLoader.so
WORKDIR /opt/htdocs
RUN usermod -u 1000 www-data
VOLUME ["/Users/lxpfigo/htdocs"]
