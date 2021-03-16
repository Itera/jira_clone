FROM node:12.18-alpine

WORKDIR /app

COPY package*.json ./
COPY tsconfig*.* ./

RUN npm ci

COPY . ./

EXPOSE 3000

RUN npm run build

CMD npm run start:production
