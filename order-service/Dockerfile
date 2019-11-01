FROM node

LABEL author="Mikael"

ENV NODE_ENV production

ENV PORT 80

ADD . /order-service

WORKDIR /order-service

RUN npm install

CMD [ "npm", "start" ]