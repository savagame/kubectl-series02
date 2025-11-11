# Kubernetes Helpful Tools
## simply clone it your pc and use it, you should have one cluster at least on your pc, this is for development, testing and learing, not production.
### kubernetes manifests for stateless, statefull applications.
```
minikube start --driver=docker
kubectl config current-context
kubectl cluster-info
kubectl apply -f application/guestbook/frontend-development.yaml
kubectl get pods --watch -l app=nginx
```

### deploy wordpress and mysql with persistent volume claim
```
minikube start --driver=docker
kubectl config current-context
kubectl cluster-info
kubectl apply -k ./
kubectl get pods
kubectl port-forward svc/wordpress 8080:80
curl http://localhost:8080
```
