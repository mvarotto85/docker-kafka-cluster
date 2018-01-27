FROM java:openjdk-8-jre

RUN mkdir -p /etc/zookeeper && mkdir -p /data/zookeeper

ADD zoo.cfg /etc/zookeeper/zoo.cfg

RUN mkdir -p /var/opt/kafka \
            && mkdir /var/opt/zookeeper \
            && cd /var/opt/kafka \
            && wget http://mirror.nohup.it/apache/kafka/1.0.0/kafka_2.12-1.0.0.tgz \
            && tar xvzf kafka_2.12-1.0.0.tgz \
            && rm kafka_2.12-1.0.0.tgz \
            && cd /var/opt/zookeeper \
            && wget http://mirror.nohup.it/apache/zookeeper/zookeeper-3.5.2-alpha/zookeeper-3.5.2-alpha.tar.gz \
            && tar xvzf zookeeper-3.5.2-alpha.tar.gz \
            && rm zookeeper-3.5.2-alpha.tar.gz \
            && touch /etc/zookeeper/nodes.cfg

