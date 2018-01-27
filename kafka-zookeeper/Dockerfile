FROM java:openjdk-8-jre

RUN mkdir -p /var/opt/kafka \
            && cd /var/opt/kafka \
            && wget http://mirror.nohup.it/apache/kafka/1.0.0/kafka_2.12-1.0.0.tgz \
            && tar xvzf kafka_2.12-1.0.0.tgz \
            && wget http://mirror.nohup.it/apache/zookeeper/zookeeper-3.5.2-alpha/zookeeper-3.5.2-alpha.tar.gz \
            && tar xvzf zookeeper-3.5.2-alpha.tar.gz \
            && rm kafka_2.12-1.0.0.tgz \
            && rm zookeeper-3.5.2-alpha.tar.gz

