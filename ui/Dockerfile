# Node image is used for building the files
FROM node:12.14.1-alpine

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY . .

# Local Installation of package
RUN yarn

# Build
RUN yarn build

# Serve the build
CMD ["yarn", "serve"]