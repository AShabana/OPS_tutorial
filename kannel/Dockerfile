FROM centos:7
MAINTAINER a.shabana@cequens.com
RUN yum -y install svn gcc glibc make libxml2-devel mariadb-devel mysql 2> /dev/null > /dev/null && echo "Pre-requists installed successfull ..."
RUN mkdir /kannel && echo "bundle root dir created .."
WORKDIR  /kannel
RUN svn co https://svn.kannel.org/gateway/trunk > /dev/null && echo "latest kannel released pulled " 
WORKDIR  /kannel/trunk
RUN pwd
RUN svn info 
RUN ./configure --with-mysql --disable-wap
RUN make > /dev/null && echo "package installed "
RUN make install 
