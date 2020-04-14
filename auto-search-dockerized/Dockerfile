FROM node:13.12.0-alpine3.10

EXPOSE 3000

RUN apk add --update tini

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

COPY package.json package.json

RUN npm install

COPY . .

CMD npm start