FROM node
LABEL maintainer="Arna, Gabriel, Nanna"

WORKDIR /app
COPY . /app


RUN npm install

ENV NODE_ENV production

ENTRYPOINT ["npm", "start"]