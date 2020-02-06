## Creating a Pod
The simplest way to create a Pod is via the imperative kubectl run command. For example, to run the kuard server, use:

`echo  "kubectl run kuard --generator=run-pod/v1  --image=gcr.io/kuar-demo/kuard-amd64:blue"`{{execute}}