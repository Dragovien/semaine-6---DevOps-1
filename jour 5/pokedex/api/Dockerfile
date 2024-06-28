FROM node:17
WORKDIR /app
COPY package.json /app
RUN npm install

ENV NODE_ENV=production

COPY . /app
EXPOSE 3000

CMD ["npm", "start"]
