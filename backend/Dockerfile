FROM node:20.9.0-alpine

WORKDIR /usr/src/app

RUN npm install -g npm@10.2.4

COPY package*.json ./

RUN apk add --no-cache git

COPY . .

RUN npm install

RUN npm install https://github.com/devzery/devzery_middleware_express

EXPOSE 8888

CMD ["npm", "run", "dev"]