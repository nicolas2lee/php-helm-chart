FROM centos/httpd-24-centos7
WORKDIR /php-dependencies
COPY ./rpm-package .
USER root
RUN yum -y localinstall **.rpm
USER default
CMD /bin/php -v