FROM adoptopenjdk:11-jdk-hotspot

COPY ./target/spring-boot-hello-world-example-0.0.1-SNAPSHOT.jar /usr/app/
 
WORKDIR /usr/app

RUN sh -c 'touch spring-boot-hello-world-example-0.0.1-SNAPSHOT.jar'

ENTRYPOINT ["java","-jar","spring-boot-hello-world-example-0.0.1-SNAPSHOT.jar"]
