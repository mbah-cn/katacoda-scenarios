## Pod Details
Sometimes, the single-line view is insufficient because it is too terse. Additionally, Kubernetes maintains numerous events about Pods that are present in the event stream, not attached to the Pod object.

To find out more information about a Pod (or any Kubernetes object) you can use the kubectl describe command. For example, to describe the Pod we previously created, you can run:

`kubectl describe pods nginx`{{execute}}
This outputs a bunch of information about the Pod in different sections. At the top is basic information about the Pod:
```
Name:           nginx
Namespace:      default
Node:           node1/x.x.x.x
Start Time:     date and time of pod creation
Labels:         <none>
Annotations:    <none>
Status:         Running
IP:             x.x.x.x
Controllers:    <none>
```
