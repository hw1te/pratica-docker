FROM node:alpine

WORKDIR /app

COPY package*.json ./

RUN npm install --only=production

COPY . .

EXPOSE 3000

ENTRYPOINT [ "sh", "-c", "npm start > var/log/frontend/logs.txt"]
