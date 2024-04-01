FROM centos:7
RUN yum update -y
RUN yum install httpd -y
EXPOSE 80
RUN rm -rvf /var/www/index.html
COPY ./Google.html /var/www/html
RUN systemctl enable httpd.service
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]

