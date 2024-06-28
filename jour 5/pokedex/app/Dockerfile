# pull official base image
FROM node:16

# set working directory
WORKDIR /app

# install app dependencies
COPY package*.json ./
RUN npm install --silent

# add app
COPY . ./

# ENV PORT 80
EXPOSE 80

# start app
CMD ["npm", "start"]
