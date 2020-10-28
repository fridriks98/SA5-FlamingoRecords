FROM node:latest
LABEL maintainer="Friðrik Snær Ómarsson"

WORKDIR /app
COPY . /app

RUN npm install

ENV NODE_ENV production
ENV PORT=80

ENV HOSTNAME message-broker
ENV RABBITMQ_USER user
ENV RABBITMQ_PASSWORD pass
ENV RABBITMQ_VHOST /  

CMD ["npm", "start"]