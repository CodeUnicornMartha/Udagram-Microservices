# Cloud Developer

## Table of Contents

* [Credentials](#credentials)
* [Docker](#docker)
* [Kubernetes](#kubernetes)


##Credentials
- set locally your environment variables
- fill in your credentials in env-secret.yaml file
- fill in your credentials in aws-secret.yaml file
- fill in your credentials in env-configmap.yaml file

## docker
Start with running the application locally:
- docker-compose -f docker-compose-build.yaml build
- docker-compose up 

## kubernetes
Deploy App to to Kubernetes Cluster
- aws eks --region <> update-kubeconfig --name <>
- kubectl get nodes
Do the following for frontend, reverseproxy, backend-feed, backend-user:
- kubectl apply -f <service-file-names>
- kubectl apply -f <deployment-file-names>
- kubectl get pods
- kubectl get svc
- kubectl get deployments






