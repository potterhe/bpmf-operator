# bpmf-operator

- 基于 [operator-sdk](https://sdk.operatorframework.io/): v1.28.1 初始化

## kubebuilder

- [kubebuilder](https://kubebuilder.io)
- [快速入门- The Kubebuilder Book - 云原生社区](https://cloudnative.to/kubebuilder/)

```sh
operator-sdk init --domain bpmf.io --repo github.com/bpmfio/bpmf-operator --plugins=go/v4-alpha
```

2023.5.21 kubebuilder 已经标准化 go/v4，但 operator-sdk 还没有完成跟进，这需要修订。

### Guestbook

`Guestbook` 是 [kubebuilder quick-start](https://kubebuilder.io/quick-start.html) 中的样例项目，实现在[guestbook-operator](https://github.com/kubernetes-sigs/kubebuilder-declarative-pattern/tree/6ba29caa6026486b7e4eb1baa27bd5d891a208e0/examples/guestbook-operator)

```sh
operator-sdk create api --group webapp --version v1 --kind Guestbook --resource --controller
```

### VisitorsApp

`VisitorsApp` 是《Kubernetes Operators》一书中的样例，该书中的示例是基于 operator-sdk 0.11.x 版本的。

```sh
operator-sdk create api --group webapp --version v1 --kind VisitorsApp --resource --controller
```