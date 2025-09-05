```sh
kubectl -n default get secret argocd-initial-admin-secret -o jsonpath="{.data.password}"
```
