# Kubernetes Minikube Task

## Files
- deployment.yaml → Defines the deployment with Nginx container
- service.yaml → Exposes the app via NodePort
- screenshots/ → Contains screenshots of outputs

## Steps to Run
```bash
minikube start --driver=docker
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl get pods
kubectl get svc
minikube service hello-service
