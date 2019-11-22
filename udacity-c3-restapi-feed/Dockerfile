FROM node:12
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
# Set access rights and switch to non-privileged user
# udacity help
# https://github.com/docker/compose/issues/4039
# Bundle app source
COPY . .
#COPY package*.json ./
RUN chown -R node:node . && chmod -R o-rwx .
USER node
# Install dependencies
RUN npm install
#RUN npm ci 

EXPOSE 8080
ENTRYPOINT [ "npm", "run", "prod" ]
