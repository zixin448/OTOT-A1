FROM node:16

# Create app directory
WORKDIR /app

# Install app dependencies
COPY package*.json ./

# If you are building your code for production
# RUN npm ci --only=production
RUN npm install

# Bundle app source
COPY . .

# map the port by docker daemon
EXPOSE 8080

CMD [ "node", "index.js" ]