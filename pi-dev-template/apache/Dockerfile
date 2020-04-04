ARG APACHE_VERSION
FROM httpd:$APACHE_VERSION
RUN apt-get update;\apt-get upgrade;
COPY custom.apache.conf /usr/local/apache2/conf/custom.apache.conf
RUN echo "Include /usr/local/apache2/conf/custom.apache.conf" \
    >> /usr/local/apache2/conf/httpd.conf
COPY server.crt /usr/local/apache2/conf/server.crt
COPY server.key /usr/local/apache2/conf/server.key