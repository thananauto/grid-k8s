# grid-k8s
sample yaml files to setup a grid infrastructure using kubernetes

In Kubernetes, a Deployment manages and scales a set of identical Pods, while a Service provides a stable network endpoint for accessing those Pods, and the number of Pods is defined by the specified number of replicas in the Deployment configuration

Before start using scalable by KEDA install by `kubectl` command
```
# Including admission webhooks
kubectl apply --server-side -f https://github.com/kedacore/keda/releases/download/v2.12.1/keda-2.12.1.yaml
# Without admission webhooks
kubectl apply --server-side -f https://github.com/kedacore/keda/releases/download/v2.12.1/keda-2.12.1-core.yaml```


Switch to namespace

```$ kubectl config set-context --current --namespace=<namespace-name>```