FROM node:16.18.1

WORKDIR /app

COPY ./package*.json ./

RUN npm install

RUN chown -R node:node /app/node_modules

COPY . ./

EXPOSE 3000

CMD ["npm", "run", "start"]