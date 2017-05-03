FROM centos:6

MAINTAINER brunomassaini@gmail.com

### Install OpenSSH
RUN yum -y install openssh-server openssh-clients
RUN chkconfig sshd on && service sshd start

### Install Apache-server
RUN yum -y install httpd mod_ssl
RUN /usr/sbin/apachectl start

EXPOSE 80 22