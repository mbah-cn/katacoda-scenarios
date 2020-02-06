In order to make the docker image available to Kubernetes we need to store the image in a docker registry. In this case, we will run a local registry using Docker.

Let's create a local docker registry by executing the following command.

`docker run -d -p 5000:5000 --restart=always --name registry registry:2`{{execute}}