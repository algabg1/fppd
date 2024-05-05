FROM openjdk:8-jdk-alpine
VOLUME /tmp
ARG JAVA_OPTS
ENV JAVA_OPTS=$JAVA_OPTS

WORKDIR /app

COPY target/demo-1.jar fppd.jar
EXPOSE 3000

ENTRYPOINT ["java", "$JAVA_OPTS", "-jar", "fppd.jar"]
