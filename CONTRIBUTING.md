基于 [operator-sdk](https://sdk.operatorframework.io/): v1.34.1 初始化

```sh
operator-sdk init --domain bpmf.io --repo github.com/bpmfio/bpmf-operator
```

### Guestbook

`Guestbook` 是 [kubebuilder quick-start](https://kubebuilder.io/quick-start.html) 中的样例项目，实现在[guestbook-operator](https://github.com/kubernetes-sigs/kubebuilder-declarative-pattern/tree/6ba29caa6026486b7e4eb1baa27bd5d891a208e0/examples/guestbook-operator)。 Kubernetes tutorials [Example: Deploying PHP Guestbook application with Redis](https://kubernetes.io/docs/tutorials/stateless-application/guestbook/) 描述了这个应用。

```sh
operator-sdk create api --group webapp --version v1 --kind Guestbook --resource --controller
```

本地测试

```sh
$ kind create cluster --name=1.28 --image=kindest/node:v1.28.0

make install run
kubectl apply -f config/samples/webapp_v1_guestbook.yaml
```