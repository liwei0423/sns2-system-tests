FROM confluentinc/cp-ksql-server:5.3.0

RUN mkdir -p /opt/kafka-ksql/jars
RUN mkdir -p /opt/kafka-ksql/scripts
RUN apt-get -y install curl
RUN curl -k -S "http://central.maven.org/maven2/no/sysco/middleware/kafka/kafka-interceptor-zipkin/0.4.2/kafka-interceptor-zipkin-0.4.2.jar" -o /opt/kafka-ksql/jars/kafka-interceptor-zipkin-0.4.2.jar
RUN ln -s /opt/kafka-ksql/jars/kafka-interceptor-zipkin-0.4.2.jar /usr/share/java/ksql-server/