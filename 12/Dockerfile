FROM ubuntu:18.04

WORKDIR /usr/src/app

RUN apt-get update && apt-get install curl -y

RUN curl -sL https://deb.nodesource.com/setup_14.x | bash

RUN apt-get install -y nodejs

COPY . .

EXPOSE 5000

RUN npm install

RUN npm run build

RUN npm install -g serve

CMD serve -s -l 5000 build