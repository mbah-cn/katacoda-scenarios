To verify the service was created, let's use kubectl to display current services

`kubectl get service`{{execute}}

Validate web application works using curl.

`curl -i [[HOST_SUBDOMAIN]]-32321-[[KATACODA_HOST]].environments.katacoda.com`{{execute}}

Or select the link below to view the we application in a browser.

https://[[HOST_SUBDOMAIN]]-[[KATACODA_HOST]].environments.katacoda.com