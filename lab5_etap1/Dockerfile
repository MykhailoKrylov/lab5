FROM node:alpine AS builder
ARG VERSION=1.0.0
ENV APP_VERSION=$VERSION
WORKDIR /usr/app
COPY ./package.json ./
RUN npm install
COPY ./index.js ./
EXPOSE 8084
CMD ["npm", "start"]
