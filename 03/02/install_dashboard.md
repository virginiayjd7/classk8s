# Kubernetes Dashboard
minikube start --force --driver=docker
## Instalar:
https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/
--
kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.6.1/aio/deploy/recommended.yaml

kubectl -n kubernetes-dashboard create token admin-user

```
kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.5.0/aio/deploy/recommended.yaml
kubectl apply -f admin_user.yaml
kubectl -n kubernetes-dashboard create token admin-user
kubectl proxy

http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/
```

## Borrar:

```
kubectl delete -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.5.0/aio/deploy/recommended.yaml
kubectl delete -f admin_user.yaml
```
