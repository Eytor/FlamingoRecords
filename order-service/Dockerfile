FROM node

LABEL author="Mikael"

ENV NODE_ENV production

ENV PORT 4000

ADD ./order-service/ /app/order-service/

WORKDIR /order-service/

RUN npm install

CMD [ "npm", "start" ]