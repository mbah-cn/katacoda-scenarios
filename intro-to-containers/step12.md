First let's make sure we are in the directory with your yaml files that describe how to manipulate Kubernetes.

`cd ~/intro-to-containers/kubernetes-yaml`{{execute}}

First, let's take a look at node-deploy.yaml. This yaml configuration is a Deployment. The most important elements to note are that we are requesting 2 copies (replicas) of the Node web application. Also, near the bottom we are defining the image (our node-web-app) we want to use and pulling it from our local repository.

`cat node-deploy.yaml`{{execute}}