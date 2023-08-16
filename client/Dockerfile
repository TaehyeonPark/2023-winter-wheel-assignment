FROM node:16-alpine

WORKDIR /usr/src/app
COPY . .

RUN npm install
RUN npm run build

EXPOSE 80
CMD ["sh", "-c", "npx react-inject-env set && serve -s build -l 80"]