FROM openjdk:8-jdk-alpine
MAINTAINER jenkins_poc
VOLUME /tmp
ARG JAVA_OPTS
ENV JAVA_OPTS=$JAVA_OPTS
COPY spring/target/springboothelloworld-0.0.1.jar springboothelloworld.jar
EXPOSE 9090
ENTRYPOINT exec java $JAVA_OPTS -jar springboothelloworld.jar
