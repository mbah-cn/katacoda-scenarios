## Check the POD status
You can see the status of this Pod by running:

`kubectl get pods`{{execute}}

You may initially see the container as Pending, but eventually you will see it transition to Running, which means that the Pod and its containers have been successfully created.

Alternatively, you can watch the pod being created by using the following command:

`kubectl get pods -w`{{execute}}