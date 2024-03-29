1. First create the deployment to spin up the pods
2. Then create the service to map the nodeport to the pods for external access
3. Then find what your node/nodes ip address is
```yaml
kubectl get nodes
kubectl describe nodes
```

4. Look for Addresses.InternalIP and do
{ip-address}:30004

# Other

If running on minikube, you can also use the

```
minikube service {your-service-name}
```