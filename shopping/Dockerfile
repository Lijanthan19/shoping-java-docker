FROM eclipse-temurin:17-jre

WORKDIR /app

COPY target/shopping-0.9.0-SNAPSHOT.jar app.jar
COPY app.yaml app.yaml
COPY applicationTags.yaml shopping/applicationTags.yaml

EXPOSE 50050
EXPOSE 50150

ENTRYPOINT ["java","-jar","app.jar","server","app.yaml"]