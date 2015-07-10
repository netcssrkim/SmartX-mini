FROM raspbian-oracle_java:1.1
MAINTAINER Seungryong Kim <srkim@nm.gist.ac.kr>

RUN sudo wget --no-check-certificate http://apache.tt.co.kr/kafka/0.8.2.0/kafka_2.10-0.8.2.0.tgz -O - | tar -zxv
#RUN sudo tar zxvf kafka-0.8.2.1-src.tgz
RUN sudo mv kafka_2.10-0.8.2.0 /kafka
#RUN sudo rm kafka-0.8.2.1-src.tgz


WORKDIR /kafka

#CMD ls -al
