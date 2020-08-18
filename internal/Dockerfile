FROM node:12.14.1-alpine

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Install app dependencies
COPY package.json .
COPY yarn.lock .
RUN yarn

# Bundle app source
COPY . .

EXPOSE 80
CMD [ "npm", "start" ]
