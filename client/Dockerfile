FROM node:14 as build

RUN apt-get update && apt-get install -y curl

WORKDIR /1169_frontend

COPY package*.json ./

RUN npm install

RUN npm install -g serve

COPY . .

RUN npm run build

EXPOSE 1169

CMD ["serve", "-s", "build"]