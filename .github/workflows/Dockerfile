FROM confluentinc/cp-server-connect:7.4.0

RUN confluent-hub install --no-prompt confluentinc/kafka-connect-jdbc:latest

USER root

RUN wget "https://repo1.maven.org/maven2/com/ibm/db2/jcc/11.5.9.0/jcc-11.5.9.0.jar"

RUN cp jcc-11.5.9.0.jar /usr/share/java/kafka-connect-jdbc

USER 1001
