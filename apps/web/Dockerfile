FROM node:20-alpine

WORKDIR /app

COPY package.json ./
RUN npm install

COPY src ./src
COPY next.config.js ./

RUN npm run build

EXPOSE 3000
CMD ["npm", "run", "start"]
