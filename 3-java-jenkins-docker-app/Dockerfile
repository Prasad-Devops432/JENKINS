# Use Eclipse Temurin OpenJDK 17 as base image
FROM eclipse-temurin:17-jdk

WORKDIR /app

COPY target/java-jenkins-docker-1.0-SNAPSHOT.jar app.jar

ENTRYPOINT ["java", "-jar", "app.jar"]
