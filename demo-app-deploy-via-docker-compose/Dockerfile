# FROM maven:3.6.0-jdk-8-alpine as BUILD
# COPY . /app
# RUN mvn -f /app/pom.xml clean package

FROM maven:3.6.0-jdk-8-alpine
COPY . /app
RUN mvn -f /app/pom.xml clean package
EXPOSE 80
CMD ["java", "-jar", "/app/target/demo-0.0.1-SNAPSHOT.jar"]