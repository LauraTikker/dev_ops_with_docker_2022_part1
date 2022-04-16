FROM ubuntu:18.04

WORKDIR /usr/src/app

COPY website-script.sh .

RUN chmod +x website-script.sh

RUN apt-get update && apt-get install curl -y

CMD ./website-script.sh 