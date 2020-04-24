FROM node:12-buster-slim

WORKDIR /usr/src/app
COPY package*.json ./
RUN npm ci

COPY . .
ENV NODE_ENV "development"
EXPOSE 3003

CMD [ "npm", "run", "container" ]