FROM robbanl/php54-fpm
ADD php.ini    /usr/local/etc/php/php.ini
COPY redis.tgz /home/redis.tgz
RUN pecl install /home/redis.tgz 
RUN echo "extension=redis.so" > /usr/local/etc/php/conf.d/redis.ini
ADD ZendGuardLoader.so /usr/local/ext/ZendGuardLoader.so
WORKDIR /opt/htdocs
RUN usermod -u 1000 www-data
VOLUME ["/Users/lxpfigo/htdocs"]

