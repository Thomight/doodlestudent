FROM openjdk:11 as build
EXPOSE 8080
WORKDIR /app
COPY . /app
# RUN apt-get install maven && mvn install
# RUN ./mvnw clean package -Dquarkus.package.type=uber-jar
CMD [ "java", "-jar", "./target/tlcdemoApp-1.0.0-SNAPSHOT-runner.jar" ]

# FROM openjdk:11
# COPY --from=build /app/target/tlcdemoApp-1.0.0-SNAPSHOT-runner.jar .