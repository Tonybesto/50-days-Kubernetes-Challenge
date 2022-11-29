FROM schoolofdevops/maven:spring as build_stage

WORKDIR /app

COPY .  .

RUN mvn spring-javaformat:apply && \
    mvn package -DskipTests && \
    mv target/spring-petclinic-2.3.1.BUILD-SNAPSHOT.jar /run/petclinic.jar


FROM adoptopenjdk/openjdk11:alpine-slim

COPY --from=build_stage /run/ .

EXPOSE 8080 

CMD java -jar petclinic.jar