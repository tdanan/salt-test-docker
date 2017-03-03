#
# Version 1

# Pull from CentOS RPM Build Image
FROM centos
MAINTAINER thomas danan <tomadanan@gmail.com>

RUN yum -y install net-tools
RUN yum -y install epel-release
RUN yum repolist
RUN yum -y install salt-minion 

# prepare conf folders
RUN mkdir -p /etc/salt/
COPY etc/minion /etc/salt/

EXPOSE 4505 4506 8080 8081

# Output
WORKDIR /home/docker
CMD salt-minion
