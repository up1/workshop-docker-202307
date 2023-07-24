# Base image
FROM node:20-alpine3.17 

# Copy file
WORKDIR /app
COPY . /app

# Download dependencies
RUN npm install

# Start server
CMD [ "npm", "start" ]
