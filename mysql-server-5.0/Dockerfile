FROM centos:5.11
RUN yum -y install mysql-server-5.0.95-5.el5_9

COPY my.cnf /etc/my.cnf
COPY initial.sql /initial.sql

RUN mysql_install_db

USER mysql

CMD ["mysqld_safe", "--init-file=/initial.sql"]

EXPOSE 3306
