FROM amazonlinux:2017.09

RUN yum -y update && \
    yum -y install \
      httpd24 \
      mysql57 \
      php56 \
      php56-mbstring \
      php56-mysqlnd \
      which \
      mod24_ssl \
      postfix && \
    yum clean all

EXPOSE 80

CMD ["/usr/sbin/apachectl", "-D", "FOREGROUND"]
