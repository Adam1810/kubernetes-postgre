Test Repo for postgres running on kubernetes

Config Maps for PostgreSQL Configurations
$ kubectl create -f postgres-configmap.yaml 

Persistent Storage Volume
$ kubectl create -f postgres-storage.yaml 

PostgreSQL Deployment
$ kubectl create -f postgres-deployment.yaml 

PostgreSQL Service
$ kubectl create -f postgres-service.yaml 

Delete PostgreSQL Deployments

kubectl delete service postgres 
kubectl delete deployment postgres
kubectl delete configmap postgres-config
kubectl delete persistentvolumeclaim postgres-pv-claim
kubectl delete persistentvolume postgres-pv-volume