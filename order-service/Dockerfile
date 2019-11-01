FROM node:latest
LABEL maintainer="Arna, Gabriel, Nanna"
 
WORKDIR /app
COPY package*.json ./
COPY . /app

RUN npm install
 
ENV NODE_ENV production
ENV PORT=80

ENTRYPOINT ["npm", "start"]
