FROM node:lts-slim

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app


COPY package*.json ./

RUN npm install
RUN npm install react-scripts@4.0.0 -g
COPY . .


EXPOSE 3000
EXPOSE 6006
CMD [ "npm", "start" ]


