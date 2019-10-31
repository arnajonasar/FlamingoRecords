FROM node
LABEL maintaner="Arna, Gabríel, Nanna"

WORKDIR /app
COPY . /app

RUN npm install

ENV NODE_ENV production

ENTRYPOINT [ "npm", "start" ]