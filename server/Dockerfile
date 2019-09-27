# Base image we are modifying from https://hub.docker.com/
FROM node:12-alpine

# Creating App Directory
RUN mkdir -p /unrama/server
WORKDIR /unrama/server

COPY package.json /unrama/server

RUN npm install

COPY . /unrama/server

# Run final command to kick off server
CMD ["npm", "run", "server"]
