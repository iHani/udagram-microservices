## Udagram Microservices
Udagram is a social media app for sharing images, refactored into Microservices and Deploy.

### Getting Started:
Start by running pods in `udacity-c3-deployment/k8s`:

```
kubectl apply -f frontend-deployment.yaml
kubectl apply -f frontend-service.yaml
kubectl apply -f backend-feed-deployment.yaml
kubectl apply -f backend-feed-service.yaml
kubectl apply -f backend-user-deployment.yaml
kubectl apply -f backend-user-service.yaml
kubectl apply -f reverseproxy-deployment.yaml
kubectl apply -f reverseproxy-service.yaml
```

Then create a kubernete cluster using `eksctl`:

`eksctl create cluster -f cluster-spec.yaml --install-vpc-controllers`

- The public GitHub repo:

    https://github.com/iHani/udagram-microservices

- Docker Hub repos:

    https://hub.docker.com/r/ihani/udacity-restapi-user
    https://hub.docker.com/r/ihani/udacity-restapi-feed
    https://hub.docker.com/r/ihani/udacity-frontend
    https://hub.docker.com/r/ihani/reverseproxy

