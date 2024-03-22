FROM centos:7
LABEL Author="Divya"
RUN yum install httpd -y
RUN yum install unzip -y
RUN rm -rf /var/www/html/*
ADD  https://www.free-css.com/free-css-templates/page292/honey  /var/www/html/
WORKDIR /var/www/html/
RUN unzip honey.zip
RUN mv honey-html/* .
EXPOSE 80
CMD httpd -DFOREGROUND