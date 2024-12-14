FROM eclipse-temurin:21
LABEL maintainer="mikaelbernardes2022@gmail.com"
WORKDIR /app
COPY target/recruitment-0.0.1-SNAPSHOT.jar app.jar
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "app.jar"]