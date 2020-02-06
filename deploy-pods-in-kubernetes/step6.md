## Listing Pods
Now that we have a Pod running, let’s go find out some more about it. Using the kubectl command-line tool, we can list all Pods running in the cluster. For now, this should only be the single Pod that we created in the previous step:

`echo "kubectl get pods"`{{execute}}


You can see the name of the Pod (kuard) that we gave it in the previous YAML file. In addition to the number of ready containers (1/1), the output also shows the status, the number of times the Pod was restarted, as well as the age of the Pod.

If you ran this command immediately after the Pod was created, you might see:
```
NAME       READY     STATUS    RESTARTS   AGE
kuard      0/1       Pending   0          1s

```

The **Pending** state indicates that the **Pod** has been submitted but hasn’t been scheduled yet.

If a more significant error occurs (e.g., an attempt to create a Pod with a container image that doesn’t exist), it will also be listed in the status field.
