# What is Docker 
  docker is a platform that allow you to create deploy and run application in lightweight container.

# Why Docker 
   "We use Docker because it solves common deployment problems. It packages applications with all
    their dependencies, so they run the same everywhere. Docker makes applications portable, efficient,
    and quick to deploy. It also simplifies managing applications by keeping them isolated in containers,
    which are lightweight and easy to scale."

# what is container ?
   "A Docker container is a lightweight, portable box that includes everything an application needs to
   run, like code and libraries. It runs in isolation, so it doesn’t affect other apps, and works the same on
   any system with Docker. This makes it fast, consistent, and resource-efficient."

# Docker Architecture 
  Docker has main three parts : 
 1. Docker Client : its what you use give command like " docker run "
 2. Docker engine : the main system that run containers, it includes the docker daemon which manage container and image 
 3. Docker registry : A place to store and pull images like docker hub.
  the client talk to the docker engine, which handles container and registry provide the images together they make it
  easy to build run and manage applicationn in container.

