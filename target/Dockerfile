# Define base docker image
FROM openjdk:20

# Copy the application JAR file into the container
ADD target/task1-0.0.1-SNAPSHOT.jar task1-0.0.1-SNAPSHOT.jar

# Set environment variables
ENV SPRING_DATA_MONGODB_URI=mongodb://mongo-db:27017/task1
ENV SPRING_PROFILES_ACTIVE=prod

# Expose the port your Spring Boot application listens on
EXPOSE 8080

# Specify the command to run application
ENTRYPOINT ["java", "-jar", "task1-0.0.1-SNAPSHOT.jar"]
