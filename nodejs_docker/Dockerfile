FROM node:12.18.1
WORKDIR /app
COPY package.json /app/
COPY package-lock.json /app/
RUN npm install
COPY . .
CMD [ "node", "server.js" ]
