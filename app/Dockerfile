FROM node:16-alpine

WORKDIR /app

COPY ./package.json ./

COPY --chown=node:node package.json .
RUN npm install -g gulp-cli
RUN npm install --legacy-peer-deps

COPY --chown=node:node . .
USER node

EXPOSE 3000
