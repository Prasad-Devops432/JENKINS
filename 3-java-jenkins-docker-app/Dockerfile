# Eclipse Temurin OpenJDK 17 base image
FROM eclipse-temurin:17-jdk

WORKDIR /app

# Run as a non-root user
RUN useradd --create-home appuser
USER appuser

# The JAR is built by Maven (mvn package) before the image is built
COPY target/java-jenkins-docker-1.0-SNAPSHOT.jar app.jar

ENTRYPOINT ["java", "-jar", "app.jar"]
