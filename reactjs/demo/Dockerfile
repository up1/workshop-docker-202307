FROM node:20-alpine3.17 AS step_1
WORKDIR /app
COPY package*.json /app
RUN npm install
COPY . /app
# /app/dist
RUN npm run build

FROM nginx
COPY --from=step_1 /app/dist /usr/share/nginx/html
