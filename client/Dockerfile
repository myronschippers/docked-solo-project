# Base image we are modifying from https://hub.docker.com/
FROM node:12-alpine

# set working directory
RUN mkdir -p /unrama/client
WORKDIR /unrama/client

# install and cache app dependencies
COPY package.json /unrama/client/package.json
RUN npm install

COPY . /unrama/client

# Run final command to kick off client build
CMD ["npm", "run", "client"]
