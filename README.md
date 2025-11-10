# Kubernetes Helpful Tools
## kubernetes manifests for stateless, statefull applications.
### simply clone it your pc and use it, you should have one cluster at least on your pc, this is for development, testing and learing, not production.
```
minikube start --driver=docker
kubectl config current-context
kubectl cluster-info
kubectl apply -f application/guestbook/frontend-development.yaml
kubectl get pods --watch -l app=nginx
...
