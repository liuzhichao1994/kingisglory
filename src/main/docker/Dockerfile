FROM openjdk:8-jdk-alpine
VOLUME /tmp
ADD kingisglory-0.0.1-SNAPSHOT.jar app.jar

#COPY ./app-entrypoint.sh /
#RUN chmod +x /app-entrypoint.sh

EXPOSE 8087

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]

#ENTRYPOINT ["/app-entrypoint.sh"]


#mvn package && java -jar target/docker-0.0.1-SNAPSHOT.jar