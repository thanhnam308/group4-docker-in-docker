__Kubernetes logging__ is a mechanism that __helps you understand what is happening inside your application__.

The logs are particularly useful for debugging problems and monitoring cluster activity. Most modern applications have some kind of logging mechanism, and container engines are designed to support logging.

In a cluster, logs should have a separate storage and lifecycle independent of nodes, pods, or containers. This concept is called __cluster-level logging__. Cluster-level logging architectures require a separate backend to store, analyze, and query logs. Kubernetes does not provide a native storage solution for log data. Instead, there are many logging solutions that integrate with Kubernetes (CloudWatch).

Get logs of a pod in k8s:
```bash
kubectl logs –f pods-name
```

Get logs of a specific container:
```bash
kubectl logs pod-name container-name
```

Get logs from a set of Pods with given label:
```bash
kubectl logs -l my-label=my-value --all-containers
```

