FROM node:18
WORKDIR /usr/src/app
COPY package*.json ./

RUN apt-get update || : && apt-get install python make g++ nano -y
RUN yarn install

COPY . .
RUN yarn build
EXPOSE 3000
CMD [ "yarn", "start" ]