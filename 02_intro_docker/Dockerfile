FROM openjdk:8u151-slim
VOLUME /tmp
ADD app.jar app.jar
RUN sh -c 'touch /app.jar'
# java.security.egd es para acelerar el calculo de numeros random
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]