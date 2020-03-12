FROM node:10.1
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY package.json /usr/src/app
RUN npm install
COPY . /usr/src/app
RUN npm run build
EXPOSE 3000
ENTRYPOINT ["npm", "run", "dev:hot"]

