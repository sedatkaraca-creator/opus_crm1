FROM node:20-alpine

WORKDIR /app

COPY package.json tsconfig.json nest-cli.json ./
RUN npm install

COPY src ./src
RUN npm run build

EXPOSE 4000
CMD ["npm", "run", "start"]
