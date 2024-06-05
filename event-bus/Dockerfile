FROM node:14

WORKDIR /1169_backend

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 4009

ENV MONGO_URL=mongodb://localhost:27017/

CMD ["node", "index.js"]
