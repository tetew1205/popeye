FROM maven:3.5-jdk-8-alpine AS builder

WORKDIR /

COPY pom.xml .

COPY src ./src

RUN mvn package

RUN mvn dependency:resolve

FROM openjdk:8-jre-alpine

CMD java -jar worker-jar-with-dependencies.jar
