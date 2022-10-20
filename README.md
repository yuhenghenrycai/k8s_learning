# k8s_learning
1. Mongo-express: web-based mongo-db admin interface written in express and node

2. There will be 2 deployments: mongo and mongo-express, each of them will have a corresponding service to load balancing request to them.

3. Mongo-service and mongo-express-service both have internal port number and target port number(port number of the deployment); Because mongo-express-service is supposed to be exposed, it should also have an external port number

4. To assign externally available IP address to mongo-express-service, run `minikube service mongo-express-service`

Notes: the params of a container like its default port number can be found in docker hub. For example [mongo-express](https://hub.docker.com/_/mongo-express)
