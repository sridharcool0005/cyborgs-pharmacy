FROM  node:boron

# Create app directory
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

RUN npm install nodemon -g

# Install app dependencies
COPY package.json /usr/src/app/
RUN npm install

# Bundle app source

COPY . /usr/src/app

EXPOSE 9001
CMD [ "npm", "start" ]

