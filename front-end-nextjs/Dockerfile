FROM node:22-alpine AS base

WORKDIR /app

COPY package.json ./
COPY package-lock.json* ./

# Souce Destinaton folder
COPY . . 

RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]
