The most important element to note is that we are creating a NodePort service and using a selector to target our node-web-app deployment. Additionally, this service will expose our application on port 32321.

We can create the service by applying the configuration using kubectl

`kubectl apply -f node-service.yaml`{{execute}}