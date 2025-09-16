FROM maven:3.9.6-amazoncorretto-21-debian AS build

WORKDIR /app
COPY pom.xml .
COPY src ./src

RUN mvn clean install -DskipTests

FROM amazoncorretto:21
WORKDIR /usr/app
COPY --from=build /app/target/service.main-0.0.1-SNAPSHOT.jar app.jar
EXPOSE 8888
CMD ["java", "-jar", "app.jar"]
