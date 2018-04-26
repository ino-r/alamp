FROM amazonlinux:2017.09

RUN yum -y update && \
    yum -y install \
      httpd24 \
      mysql57 \
      php56 \
      php56-mysqlnd \
      which && \
    yum clean all

EXPOSE 80

CMD ["/usr/sbin/apachectl", "-D", "FOREGROUND"]
