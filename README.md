EMQTT-K8S
=========

#### How to:

```
kubectl create namespace emqtt
kubectl apply -f emqtt.yaml
```

done, you should now have a emqtt cluster of 2 nodes running on kubernetes, to verify:

```
kubectl port-forward -n emqtt emqtt-0 8080:18083
```

on your browser enter ```http://localhost:8080``` to get into emqtt dashboard.
