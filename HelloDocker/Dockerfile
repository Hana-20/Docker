# Use a Java runtime as a parent image
FROM maven:3-openjdk-17-slim as build

# Set the working directory to /app
WORKDIR /app

# Copy the frontend application files to the container at /app
COPY . /app

# Expose port 8080 for the frontend application
EXPOSE 8080

# Define the command to run the frontend application
CMD ["java", "-jar", "/app/frontend.jar"]




# # Use a base image that has Java installed
# FROM maven:3-openjdk-17-slim as build

# # Set the working directory to /app
# WORKDIR /app

# # Copy the project files into the container
# COPY . /app

# # Build the project with Maven
# RUN mvn -f /app/pom.xml clean package 

# # Set the command to run the application
# CMD ["java", "-jar", "/app/target/hello world.jar"]