# Specifying on what to build the image
FROM node

# Telling docker to eecute all the commands in app folder. Or else npm i will be made run, but in root folder.
# So specifying for once and all
WORKDIR /app

# Copy all the contents from root folder to a folder named app in container, as app is our workdir
COPY . /app

RUN npm i

# All of commands above this will be made run when creating image

# Letting docker know, that we have to expose a port{80} outside the container, prior to starting work in container 
EXPOSE 80

# This will be executed when container is made run
CMD ["node","server.js"]  