FROM node:12.18-alpine

WORKDIR /app

COPY package*.json .

RUN npm config set loglevel warn

RUN npm ci

COPY . .

RUN npm run build

CMD npm run start:production
