FROM maven:3-openjdk-17-slim as build
WORKDIR /app
COPY . .
RUN mvn clean package


FROM tomcat:7-jdk8
COPY --from=build /app/target/helloDocker.war /usr/local/tomcat/webapps/
EXPOSE 8080
CMD ["catalina.sh", "run"]