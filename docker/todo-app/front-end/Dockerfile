FROM node:14-alpine

WORKDIR /app

COPY package*.json ./

RUN npm install

ADD node_modules.tar.gz ./app/node_modules

COPY . .

EXPOSE 3000

ENTRYPOINT ["npm", "start"]

