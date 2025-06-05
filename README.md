# wol
wol for my machines

# for docker

```shell
$ docker compose up -d
```

# for k8s

## require

- installed kubectl
- setting up kubeconfig

## deploy

```shell
$ cd k8s
$ kubectl apply -f namespace.yaml
namespace/gptwol created

$ kubectl kustomize --load-restrictor LoadRestrictionsNone | kubectl apply -f -
configmap/gptwol-computers-cg2cf4m85m created
service/gptwol-service unchanged
deployment.apps/gptwol-deployment created
```
