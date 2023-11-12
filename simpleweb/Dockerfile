# Specify a base image
FROM node:14-alpine

# Setup working directory
WORKDIR /usr/app

# Copy package.json to container to avoid unnecessary re-builds
COPY ./package.json ./

# Install some dependencies
RUN npm install

# Copy all the project files to container
COPY ./ ./

# Default command
CMD ["npm", "start"]
