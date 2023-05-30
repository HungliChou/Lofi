FROM node:14

# Create app directory
WORKDIR /app

COPY client ./

WORKDIR /app/client

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
RUN npm install

EXPOSE 3000

CMD [ "npm", "run", "serve" ]