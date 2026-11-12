FROM amazoncorretto:8-jdk
WORKDIR /app

COPY .mvn/ .mvn/
COPY pom.xml mvnw .
COPY src ./src

RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]
