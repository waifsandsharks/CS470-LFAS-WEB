# using Node v10
FROM node:10

# create app directory
WORKDIR /usr/src/lafs

# Install dependencies
COPY package*.json ./

RUN npm install -g @angular/cli@v6-lts
RUN npm install

# bundle app source
COPY . .

# expose port 4200 oustide container
EXPOSE 4200

# start the application
CMD ng serve --host 0.0.0.0
