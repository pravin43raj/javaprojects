FROM adoptopenjdk:11-jdk-hotspot

COPY ./target/spring-boot-0.0.1-SNAPSHOT.jar /usr/app/
 
WORKDIR /usr/app

RUN sh -c 'touch spring-boot-0.0.1-SNAPSHOT.jar'

ENTRYPOINT ["java","-jar","spring-boot-0.0.1-SNAPSHOT.jar"]
