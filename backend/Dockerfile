# It will pull node:18-alpine as the base image from Docker Hub
FROM --platform=linux/amd64 node:18-alpine
# It creates the container working directory named `node`
WORKDIR /app
# It copies all the dependencies and libraries to the working directory
COPY package.json .
COPY .env .
#It installs all the dependencies and libraries to the container
RUN npm install
#It copies all the source code and configuration files to the container working directory
COPY . .
#it exposes and runs the container to port 3333
EXPOSE 3333
#It is the command to start and run the container for the Node.js application
CMD ["node", "index.js"]