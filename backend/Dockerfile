FROM node:lts-buster-slim AS development

# Create app directory
WORKDIR /usr/src/app

COPY . /usr/src/app

RUN npm ci

EXPOSE 3030

CMD [ "npm", "run", "dev" ]

