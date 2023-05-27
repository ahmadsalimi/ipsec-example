FROM centos:7

RUN yum makecache fast
RUN yum install openswan lsof sysvinit-tools -y

COPY ./entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
