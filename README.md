scratch repo to capture process for jenkins on k8s

```console
kubectl create ns jenkins
```

```console
kubectl create -f jenkins-deployment.yaml --namespace=jenkins
```

```console
kubectl port-forward -n jenkins jenkins-deployment-7d6fff6846-btlbp 8080:8080
```
---

* todo: activate the k8s plugin under the jenkins "config" section "add cloud" to get dynamic workers/executors
* todo: remove master executors
