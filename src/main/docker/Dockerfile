FROM openjdk:8u131-jdk-alpine

WORKDIR /usr/local/bin/

#Transfer JAR-file
# COPY ./target/fleetman-0.0.1-SNAPSHOT.jar webapp.jar
COPY maven/fleetman-0.0.1-SNAPSHOT.jar webapp.jar

EXPOSE 8080

CMD ["java", "-Dspring.profiles.active=docker-demo", "-jar", "webapp.jar"]

ARG BUILD_DATE

LABEL build-date = $BUILD_DATE
LABEL maintainer = "patrick Steens / git.patje.stinch@gmail.com"
