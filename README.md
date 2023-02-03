# operator-helm
Instaclustr Kubernetes Operator helm repository

## TL;DR

```bash
$ helm repo add operator-chart https://instaclustr.github.io/operator-helm
$ helm search repo operator-chart
$ helm install my-release operator-chart/<chart> \
  --set USERNAME=${USER_NAME} --set APIKEY=${API_KEY} \
  --set HOSTNAME=${HOST_NAME} -n ${OPERATOR_NAMESPACE} --create-namespace
```
