FROM openjdk:8

WORKDIR /usr/src/app

COPY . .

EXPOSE 8080

RUN ./mvnw package

CMD java -jar ./target/docker-example-1.1.3.jar