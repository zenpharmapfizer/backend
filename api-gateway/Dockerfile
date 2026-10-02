# This is a multi-stage Dockerfile for building and running the API Gateway service.
# The first stage uses Maven to build the application, and the second stage uses a lightweight JRE image to run the application.
FROM eclipse-temurin:17-jre
WORKDIR /app
RUN groupadd -r pharma && useradd -r -g pharma pharma
COPY target/*.jar app.jar
USER pharma
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "-Djava.security.egd=file:/dev/./urandom", "app.jar"]
