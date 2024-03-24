operator-sdk: v1.34.1

```
operator-sdk init --domain bpmf.io --repo github.com/bpmfio/bpmf-operator

operator-sdk create api --group webapp --version v1 --kind Guestbook --resource --controller
```