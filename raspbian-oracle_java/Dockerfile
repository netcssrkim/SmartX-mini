FROM resin/rpi-raspbian:wheezy
MAINTAINER Seungryong Kim <srkim@nm.gist.ac.kr>

RUN apt-get update
RUN apt-get -y install wget

RUN sudo mkdir -p /opt
RUN sudo wget --no-check-certificate http://www.java.net/download/jdk8u60/archive/b21/binaries/jdk-8u60-ea-bin-b21-linux-arm-vfp-hflt-23_jun_2015.tar.gz
RUN sudo tar zxvf jdk-8u60-ea-bin-b21-linux-arm-vfp-hflt-23_jun_2015.tar.gz -C /opt
RUN sudo rm jdk-8u60-ea-bin-b21-linux-arm-vfp-hflt-23_jun_2015.tar.gz

#RUN sudo echo "export JAVA_HOME=/opt/jdk1.8.0_60" >> ~/.bashrc
#RUN sudo echo "export PATH=$PATH:$JAVA_HOME/bin" >> ~/.bashrc

ENV JAVA_HOME /opt/jdk1.8.0_60
ENV PATH $PATH:/opt/jdk1.8.0_60/bin
RUN ln -s /opt/jdk1.8.0_60/bin/java /usr/bin/java

#RUN apt-get -y install source
#RUN ["source","~/.bashrc"]
#RUN source ~/.bashrc
#RUN . ~/.bashrc

#CMD java -version
#CMD echo Hi
