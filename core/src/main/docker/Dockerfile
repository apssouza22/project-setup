FROM openjdk:11-jre-slim-stretch

ENV SPRING_OUTPUT_ANSI_ENABLED=ALWAYS \
    JHIPSTER_SLEEP=0 \
    JAVA_OPTS=""

# Add a jhipster user to run our application so that it doesn't need to run as root
RUN adduser -D -s /bin/sh apssouza
WORKDIR /home/apssouza

ADD entrypoint.sh entrypoint.sh
RUN chmod 755 entrypoint.sh && chown apssouza:apssouza entrypoint.sh
USER apssouza

ENTRYPOINT ["./entrypoint.sh"]

EXPOSE 8080

ADD *.war app.war

