FROM node:16-alpine

WORKDIR /usr/src/app

COPY ./package.json .

RUN npm install

COPY . .

RUN REACT_APP_BACKEND_URL=http://localhost:8080 npm run build

RUN npm install -g serve

EXPOSE 5000

CMD ["serve", "-s", "-l", "5000", "build"]