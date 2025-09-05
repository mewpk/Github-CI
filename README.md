```sh
kubectl -n default get secret argocd-initial-admin-secret -o jsonpath="{.data.password}"
kubectl port-forward service/my-argo-cd-argocd-server -n default 8080:443
```
