FROM openjdk:17-jdk-slim
ARG JAR_FILE=target/service1-0.0.1-SNAPSHOT.jar
COPY ${JAR_FILE} service1.jar
ENTRYPOINT ["java", "-jar", "/service1.jar"]
