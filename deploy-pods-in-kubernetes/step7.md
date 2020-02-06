## Pod Details
Sometimes, the single-line view is insufficient because it is too terse. Additionally, Kubernetes maintains numerous events about Pods that are present in the event stream, not attached to the Pod object.

To find out more information about a Pod (or any Kubernetes object) you can use the kubectl describe command. For example, to describe the Pod we previously created, you can run:

`echo "kubectl describe pods kuard"`{{execute}}
This outputs a bunch of information about the Pod in different sections. At the top is basic information about the Pod:
```
Name:           kuard
Namespace:      default
Node:           node1/10.0.15.185
Start Time:     date and time of pod creation
Labels:         <none>
Annotations:    <none>
Status:         Running
IP:             192.168.199.238
Controllers:    <none>
```
