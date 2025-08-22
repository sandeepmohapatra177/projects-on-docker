FROM node:12.2.0-alpine

WORKDIR /node

COPY . .

RUN npm install #install dependencies

RUN npm run test #run tests during build

EXPOSE 8000 
#expose the app port

CMD ["node", "app.js"]

