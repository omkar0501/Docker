# here are some common base images 
   FROM ubuntu
   
 
   FROM node    - which is pulls nodej.s lastest version 
   
   FROM node:latest - also he pulls nodej.s latest version 
   
   FROM node:18  - which is pulls nodej.s 18 version 

  
   
   FROM openjdk - which is pulls java latest version 
   
   FROM openjdk:latest - also pulls java latest version 

   FROM openjdk:17  -which is pulls java 17 version


  # Sets the working directory 
  WORKDIR /app    
  using WORKDIR /app and storing all your application files in the /app directory 

  # Copies files into the /app directory.
  COPY . .
  .. means 
    First . (Source):
    Refers to the current directory on your host machine (where the Dockerfile is located).

   Second . (Destination):
   Refers to the current working directory inside the container (set by the WORKDIR instruction or defaults to /app).

   also we use 

   COPY . /app

# install dependencies 
RUN npm install

# use EXPOSE 
EXPOSE 3000

use EXPOSE 3000 if your application runs on port 3000 inside the container.

# USE CMD 
CMD ["npm", "start"]

CMD ["npm", "start"] instruction in a Dockerfile specifies the default command to run when a container starts


# it is my docker file 
 
FROM node:16   # Use a Node.js base image

WORKDIR /app   # Set the working directory inside the container

COPY . .       # Copy all files from the current directory to /app in the container

EXPOSE 3000    # Document that the app listens on port 3000

CMD ["npm", "start"]  # Run "npm start" when the container starts





   
   

   
