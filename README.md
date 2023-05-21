# bpmf-operator

operator-sdk: v1.28.1

```sh
operator-sdk init --domain bpmf.io --repo github.com/bpmfio/bpmf-operator --plugins=go/v4-alpha
```

### Guestbook

```sh
operator-sdk create api --group webapp --version v1 --kind Guestbook --resource --controller
```

### VisitorsApp

```sh
operator-sdk create api --group webapp --version v1 --kind VisitorsApp --resource --controller
```