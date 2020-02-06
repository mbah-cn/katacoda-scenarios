## Creating a Pod Manifest
Pod manifests can be written using YAML or JSON, but YAML is generally preferred because it is slightly more human-editable and has the ability to add comments. Pod manifests (and other Kubernetes API objects) should really be treated in the same way as source code, and things like comments help explain the Pod to new team members who are looking at them for the first time.

Pod manifests include a couple of key fields and attributes: namely a **metadata section** for describing the Pod and its labels, a **spec section** for describing volumes, and a list of containers that will run in the Pod.
Navigate to the ~/depoly-pods-in-kubernetes/pod-manifests/ directory
`cd ~/depoly-pods-in-kubernetes/pod-manifests/ && ls`{{execute}}

Cat the kuard-pod.yaml to inspect its content:
`cat kuard-pod.yaml`{{execute}}
