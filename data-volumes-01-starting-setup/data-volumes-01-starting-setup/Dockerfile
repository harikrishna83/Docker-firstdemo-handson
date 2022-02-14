FROM node:14

WORKDIR /app

RUN npm install -g nodemon

COPY package.json .

RUN npm install

COPY . .

ARG DEFAULT_PORT=80

ENV PORT $DEFAULT_PORT

#VOLUME [ "/temp"]

EXPOSE $PORT

CMD [ "npm", "start"]