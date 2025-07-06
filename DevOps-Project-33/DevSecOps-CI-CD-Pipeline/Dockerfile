#FROM openjdk:21
#COPY target/*.jar app.jar
#ENTRYPOINT ["java", "-jar", "app.jar"]
# Use a lightweight official OpenJDK base image
FROM openjdk:21-jdk-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the jar file from the build context to the container
COPY target/*.jar app.jar

# Expose the port your application listens on (change if needed)
EXPOSE 8080

# Set environment variables (optional)
# ENV JAVA_OPTS=""

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
