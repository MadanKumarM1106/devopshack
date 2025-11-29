# Dockerfile for the Express server
FROM node:18-alpine AS build
WORKDIR /app

# Copy package files and install
COPY package*.json ./
RUN npm install --production

# Copy source
COPY . .

EXPOSE 5000

CMD [ "node", "server.js" ]
