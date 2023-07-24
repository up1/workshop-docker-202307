# Base image
FROM node:20-alpine3.17 

# Copy file
WORKDIR /app
COPY package*.json /app

# Download dependencies
RUN npm install

COPY . /app

EXPOSE 3000

# Start server
CMD [ "npm", "start" ]
