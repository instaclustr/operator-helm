# operator-helm
Instaclustr Kubernetes Operator helm repository

## TL;DR

```bash
$ kubectl apply -f https://github.com/cert-manager/cert-manager/releases/download/v1.10.0/cert-manager.yaml
$ helm repo add operator-chart https://instaclustr.github.io/operator-helm
$ helm search repo operator-chart
$ helm install my-release operator-chart/<chart> \
  --set USERNAME=${USER_NAME} --set APIKEY=${API_KEY} \
  --set HOSTNAME=${HOST_NAME} -n ${OPERATOR_NAMESPACE} --create-namespace
```
You can add `--set image.tag=${IMG_TAG}` to helm install command if you want to use special version. 
Latest version install by default

## Links

- Operator repository [here](https://github.com/instaclustr/operator)
- Examples of specifications for different resources [here](https://github.com/instaclustr/operator/tree/main/config/samples)
- Documentation [here](https://github.com/instaclustr/operator/tree/main/doc)
