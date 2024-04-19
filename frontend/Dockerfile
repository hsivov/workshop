# Create image based on the official Node image from dockerhub
FROM node:lts-alpine

# Create app directory
WORKDIR /usr/src/app

# Get all the code needed to run the app
COPY . /usr/src/app

# Install dependecies
#RUN npm set progress=false \
#    && npm config set depth 0 \
#    && npm i install
RUN npm ci

# Expose the port the app runs in
EXPOSE 3000

# Serve the app
CMD ["npm", "start"]
