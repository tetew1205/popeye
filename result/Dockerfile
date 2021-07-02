FROM node:12-alpine

COPY views ./views

COPY server.js .

COPY package.json .

EXPOSE 80

ENV port=80

RUN npm install

CMD npm start