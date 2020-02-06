## Creating a Pod
The simplest way to create a Pod is via the imperative kubectl run command. For example, let's run a simple nginx pod:

`kubectl run nginx --generator=run-pod/v1 --image=nginx`{{execute}}
