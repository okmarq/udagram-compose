FROM node:13
#Create app directory
WORKDIR /usr/src/app
#Install all dependencies
#A wildcard is used to ensure both package.json and package.lock.json are copied when available (npm@5+)
COPY package*.json ./
RUN npm ci
#Bundle app source
COPY . .
EXPOSE 8080
CMD [ "npm", "run", "prod" ]
