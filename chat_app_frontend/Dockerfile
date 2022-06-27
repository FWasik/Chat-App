FROM node:16.14.0-alpine

WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH

COPY package.json ./
COPY package-lock.json ./

RUN npm install -g npm@8.5.2 --silent
RUN npm install react-scripts

COPY . ./

#CMD ["npm", "start"]