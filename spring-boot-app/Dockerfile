# You can change this base image to anything else
# Use Eclipse Temurin (AdoptOpenJDK successor) with Java 17 and Alpine base
FROM eclipse-temurin:17-jre-alpine

# Define the artifact path
ARG artifact=target/spring-boot-web.jar

# Set working directory inside the container
WORKDIR /opt/app

# Copy the JAR file into the container
COPY ${artifact} app.jar

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
