# bpmf-operator

基于 [operator-sdk](https://sdk.operatorframework.io/): v1.28.1 初始化

```sh
operator-sdk init --domain bpmf.io --repo github.com/bpmfio/bpmf-operator --plugins=go/v4-alpha
```

### Guestbook

`Guestbook` 是 [kubebuilder quick-start](https://kubebuilder.io/quick-start.html) 中的样例项目，实现在[guestbook-operator](https://github.com/kubernetes-sigs/kubebuilder-declarative-pattern/tree/6ba29caa6026486b7e4eb1baa27bd5d891a208e0/examples/guestbook-operator)

```sh
operator-sdk create api --group webapp --version v1 --kind Guestbook --resource --controller
```

### VisitorsApp

```sh
operator-sdk create api --group webapp --version v1 --kind VisitorsApp --resource --controller
```