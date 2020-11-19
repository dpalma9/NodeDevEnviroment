ARG version=latest
FROM node:${version}
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies
#COPY package*.json ./
RUN npm install
COPY . .
ENTRYPOINT ["/bin/sleep", "infinity"]
