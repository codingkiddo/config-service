FROM eclipse-temurin:17
WORKDIR workspace
ARG JAR_FILE=target/config-service-0.0.1-SNAPSHOT.jar
COPY ${JAR_FILE} config-service.jar
ENTRYPOINT [ "java", "-jar", "config-service.jar" ]