# introduction

Assume you have two services those are based on `microservices` architecture. Service names are `dev` and `ops`. 
ops service has a function which validate phone no. If valid phone no it returns `YES`, for invalid phone no it 
returns `NO`. dev services needs to communicate with ops service to validate the phone no's. dev service sends 
phone no's to ops service. ops service validate them and send response back to dev service.

![Alt text](devops.png?raw=true "devops architecture")

# todo's

dev and ops services needs to communicate via `kafka`. dev service sends phone no to ops service(via kafka).
ops service validates phone no and send response back to dev service(via kafka). Develop dev and ops service
with any language(`golang/scala/python` would be prefer). Try to integrate these services with `docker`
