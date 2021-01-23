FROM openjdk:8
RUN  apt-get update && apt-get install netcat-openbsd
#RUN apk add --update netcat-openbsd && rm -rf /var/cache/apk/*
RUN mkdir -p /usr/local/authenticationservice
ADD @project.build.finalName@.jar /usr/local/authenticationservice/
ADD run.sh run.sh
RUN chmod +x run.sh
CMD ./run.sh
