## Running Pods
In the previous step, we created a Pod manifest that can be used to start a Pod running nginx. Use the kubectl apply command to launch a single instance of nginx:

`kubectl apply -f nginx-pod.yaml`{{execute}}

The Pod manifest will be submitted to the Kubernetes API server. The Kubernetes system will then schedule that Pod to run on a healthy node in the cluster, where it will be monitored by the kubelet daemon process. Don’t worry if you don’t understand all the moving parts of Kubernetes right now.
