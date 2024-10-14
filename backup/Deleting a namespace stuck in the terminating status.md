```bash
kubectl patch ns <namespace> -p '{"metadata":{"finalizers": null }}'
```