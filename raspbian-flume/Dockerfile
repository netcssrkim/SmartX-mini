FROM raspbian-oracle_java:1.0
MAINTAINER Seungryong Kim <srkim@nm.gist.ac.kr>

RUN sudo wget --no-check-certificate http://www.apache.org/dist/flume/1.6.0/apache-flume-1.6.0-bin.tar.gz -O - | tar -zxv
RUN sudo mv apache-flume-1.6.0-bin /flume
#RUN sudo rm apache-flume-1.6.0-bin.tar.gz

ADD plugins.d /flume/plugins.d
ADD flume-conf.properties /flume/conf/

RUN sudo ln -s /opt/jdk1.8.0_60/bin/java /usr/bin/java

#ENV JAVA_HOME /opt/jdk1.8.0_60
#ENV PATH $PATH:/opt/jdk1.8.0_60/bin

WORKDIR /flume

#CMD ls -al
#CMD sudo bin/flume-ng agent --conf conf --conf-file conf/flume-conf.properties --name agent -Dflume.root.logger=INFO,console

