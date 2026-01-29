# Use Java 17 JRE runtime
FROM eclipse-temurin:17-jre-alpine

# Artifact to copy
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

# Copy built JAR from Jenkins workspace
COPY ${artifact} app.jar

# Run the Spring Boot app
ENTRYPOINT ["java","-jar","app.jar"]
