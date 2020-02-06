## Running Commands in Your Container with exec
Sometimes logs are insufficient, and to truly determine what’s going on you need to execute commands in the context of the container itself. To do this you can use:

`kubectl exec nginx date`{{execute}}

You can also get an interactive session by adding the -it flags:

`kubectl exec -it nginx --  bash`{{execute}}

Type exit to exit the container interactive session:

`exit`{{execute}}
