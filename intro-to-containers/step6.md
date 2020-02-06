With the docker image created, we now can tell the docker runtime to run our container.  Notice the run command specifies a port, 49160, that will be accessible on this server. The application is, however, still listening on port 8080.

`docker run -p 49160:8080 -d node-web-app`{{execute}}