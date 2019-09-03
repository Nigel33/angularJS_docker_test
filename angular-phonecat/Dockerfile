FROM node:lts-alpine
RUN npm install -g http-server

WORKDIR /app
COPY package*.json ./

COPY . .

RUN npm install && \
    npm run start

EXPOSE 8000

CMD [ "http-server", "dist" ]