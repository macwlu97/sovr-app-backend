FROM openjdk:17-jdk-slim

# Install git
RUN apt-get update && apt-get install -y git && rm -rf /var/lib/apt/lists/*

# Set path to jar file
ARG JAR_FILE=target/config-server-0.0.1-SNAPSHOT.jar

# copy jar file to container
COPY ${JAR_FILE} config-server.jar

# run app
ENTRYPOINT ["java", "-jar", "/config-server.jar"]
