FROM node:16-alpine

WORKDIR /usr/src/app
COPY . .

RUN apk update && apk add curl
# RUN npm install cross-env -g
# RUN npm install cross-env
# RUN npm install
RUN npm ci

EXPOSE 80
ENV PORT 80
CMD ["npm", "run", "serve"]