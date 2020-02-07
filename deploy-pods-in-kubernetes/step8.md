## Deleting a Pod
When it is time to delete a Pod, you can delete it either by name:

`kubectl delete pods/nginx`{{execute}}

You can also use the same file that you used to create it:

`kubectl delete -f nginx-pod.yaml`{{execute}}

When a Pod is deleted, it is not immediately killed. Instead, if you run kubectl get pods you will see that the Pod is in the *Terminating* state. All Pods have a termination grace period. By default, this is 30 seconds. When a Pod is transitioned to Terminating it no longer receives new requests. In a serving scenario, the grace period is important for reliability because it allows the Pod to finish any active requests that it may be in the middle of processing before it is terminated.
