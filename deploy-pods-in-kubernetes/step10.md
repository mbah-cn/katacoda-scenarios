## Access your Pod
Now that your Pod is running, you’re going to want to access it for a variety of reasons. You may want to load the web service that is running in the Pod. You may want to view its logs to debug a problem that you are seeing, or even execute other commands in the context of the Pod to help debug. The following sections detail various ways that you can interact with the code and data running inside your Pod.

### Using Port Forwarding
Later in the book, we’ll show how to expose a service to the world or other containers using load balancers⁠—but oftentimes you simply want to access a specific Pod, even if it’s not serving traffic on the internet.

To achieve this, you can use the port-forwarding support built into the Kubernetes API and command-line tools.

When you run:

`kubectl port-forward nginx 8080:8080`{{execute}}

a secure tunnel is created from your local machine, through the Kubernetes master, to the instance of the Pod running on one of the worker nodes.

As long as the port-forward command is still running, you can access the Pod (in this case the kuard web interface) at
[http://localhost:8080](https://[[HOST_SUBDOMAIN]]-8080-[[KATACODA_HOST]].environments.katakoda.com/)


