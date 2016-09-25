FROM nginx:1.9
ADD  nginx.conf      /etc/nginx/nginx.conf
ADD  pathinfo.conf   /etc/nginx
ADD  php_fcgi.conf   /etc/nginx
RUN  mkdir /opt/htdocs && mkdir /opt/log && mkdir /opt/log/nginx && mkdir /etc/nginx/vhosts
ADD  test.conf     /etc/nginx/vhosts/test.conf
ADD  ll.conf      /etc/nginx/vhosts/ll.conf
ADD  lang.conf      /etc/nginx/vhosts/lang.conf
ADD  laravel.conf      /etc/nginx/vhosts/laravel.conf
ADD  ink.conf      /etc/nginx/vhosts/ink.conf
ADD  langwan.conf      /etc/nginx/vhosts/langwan.conf
RUN  chown -R www-data.www-data /opt/htdocs /opt/log
VOLUME ["/Users/lxpfigo/htdocs"]
