FROM node:10.1-alpine
ENV NODE_ENV production
WORKDIR /usr/src/app
COPY ["package.json", "package-lock.json*", "npm-shrinkwrap.json*", "./"]
# RUN npm install --production --silent && mv node_modules ../
RUN npm install --production --silent
COPY . .
EXPOSE 3000
ENTRYPOINT [ "npm", "start" ]