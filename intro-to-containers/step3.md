## Running the Docker image

In the Dockerfile, we can see that that the we are building the container from a base docker image (FROM node:10) copying files to a working directory, running the node application and exposing port 8080.

`cat Dockerfile \n`{{execute}}