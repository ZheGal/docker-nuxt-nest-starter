FROM node:18
WORKDIR /usr/src/app
COPY package*.json ./

RUN apt-get update && apt-get install -y nano
RUN yarn install

COPY . .
EXPOSE 3000
CMD [ "yarn", "start" ]