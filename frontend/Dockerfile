FROM node:16

RUN apt-get update

RUN apt-get install vi git unzip -y

RUN apt-get update && apt-get install -y \
    vi \
    git \
    unzip \
    wget

ARG NODE_ENV=development

ENV NODE_ENV=${NODE_ENV}

WORKDIR /opt/

COPY ./package.json ./yarn.lock ./

ENV PATH /opt/node_modules/.bin:$PATH

RUN yarn install

WORKDIR /opt/app

COPY ./ .

RUN yarn build

ENV HOST 0.0.0.0

EXPOSE 3000

CMD ["yarn", "dev"]