FROM node:20
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install
# ENV are in docker compose
CMD ["node", "server.js"]