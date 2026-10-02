# This is a multi-stage Dockerfile for building and running the API Gateway service.
<<<<<<< HEAD
# The first stage uses Maven to build the application, and the second stage uses a lightweight JRE image to run the application.
=======
>>>>>>> f0b19f7bcb74a4151a758ae2e760ea874e3a2993
FROM eclipse-temurin:17-jre
WORKDIR /app
RUN groupadd -r pharma && useradd -r -g pharma pharma
COPY target/*.jar app.jar
USER pharma
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "-Djava.security.egd=file:/dev/./urandom", "app.jar"]
