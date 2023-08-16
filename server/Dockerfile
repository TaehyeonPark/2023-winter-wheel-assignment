FROM node:16-alpine

WORKDIR /usr/src/app
COPY . .

RUN apk update && apk add curl
RUN npm install --save

EXPOSE 80
ENV PORT 80
CMD ["npm", "run", "serve"]