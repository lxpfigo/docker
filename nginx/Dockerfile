FROM nginx:1.9
ADD  nginx.conf      /etc/nginx/nginx.conf
ADD  pathinfo.conf   /etc/nginx
ADD  php_fcgi.conf   /etc/nginx
RUN  mkdir /opt/htdocs && mkdir /opt/log && mkdir /opt/log/nginx && mkdir /etc/nginx/vhosts
ADD  test.conf     /etc/nginx/vhosts/test.conf
ADD  imh.conf     /etc/nginx/vhosts/imh.conf
ADD  ncshop.conf     /etc/nginx/vhosts/ncshop.conf
ADD  xiaoyaochezhu.conf     /etc/nginx/vhosts/xiaoyaochezhu.conf
ADD  ink.conf     /etc/nginx/vhosts/ink.conf
RUN  chown -R www-data.www-data /opt/htdocs /opt/log
VOLUME ["/Users/lxpfigo/htdocs"]
