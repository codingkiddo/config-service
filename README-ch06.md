docker build --build-arg JAR_FILE=target/config-service-0.0.6-SNAPSHOT.jar -t config-service .


docker push ghcr.io/codingkiddo/config-service:0.0.6-SNAPSHOT