FROM node:15.14-alpine

WORKDIR /node/app

EXPOSE 3000

# RUN mkdir -p /app/node_modules/.cache && chmod -R 777 /app/node_modules/

COPY package.json package-lock.json ./

RUN npm install --silent

COPY --chown=node:node . ./

CMD ["npm", "run", "start"]