FROM node:14.17-alpine

WORKDIR /app

COPY ["package.json", "yarn.lock", "./"]

RUN yarn install

COPY . .

RUN yarn build

ENV NODE_ENV=production

EXPOSE 3333

CMD [ "yarn", "production" ]