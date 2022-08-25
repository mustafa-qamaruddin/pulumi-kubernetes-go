# Pulumi Kubernetes GoLang

```shell
minikube start
cat ~/.kube/config
kubectl get pods -A
brew install pulumi/tap/pulumi
pulumi new kubernetes-go --force
pulumi up
pulumi config set isMinikube true
pulumi up
kubectl get pods -A
kubectl get svc -A
kubectl get deployments -A
kubectl port-forward svc/nginx-93c47c4c 8080:80
curl http://localhost:8080
pulumi stack output ip
curl $(pulumi stack output ip)
pulumi destroy
pulumi stack rm dev
kubectl get pods -A
```

Reference: [https://www.pulumi.com/docs/get-started/kubernetes/](https://www.pulumi.com/docs/get-started/kubernetes/)
