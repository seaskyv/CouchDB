# CouchDB
Delpoy CouchDB with single podon Kubernetes.

couchdb-dep.yaml will create


   2 PVs with storageclass and HostPath, on Minikubes /data directory
   2 PVCs for configuration and data of CouchDB
   Service type is NodePort to expose the CouchDB port
   CouchDB deployment with single pod
   admin username and password for the CouchDB are admin:password, which pass and ENV variable to container.

To access CouchDB externally from minikube, expose the service :

$ minikube service couchdb

$ minikube service list



