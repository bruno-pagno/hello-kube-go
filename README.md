# About

This project is a "Hello world" in Kubernetes implementing a Golang web server.

## Docker image

Image name on DockerHub: `bpagno/hello-kube-go`

## Docker commands

```bash
# Build the image
docker build -t bpagno/hello-kube-go:1.0 .
# Push the image to the DockerHub
docker push bpagno/hello-kube-go:1.0
```

## Kubernetes Cluster commands

Starting the Minikube cluster

```bash
minikube start
```

### Applying the deployment & service using Kubectl

```bash
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
```

## Accessing the service

```bash
minikube service hello-kubernetes-service
```
