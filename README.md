# prepare-k8s-env
[![LICENSE](https://img.shields.io/github/license/freenet-actions/k8s-login-action)](https://github.com/freenet-actions/k8s-login-action/blob/main/LICENSE)

This action implements the Kubernetes (K8s) cluster registration and installs Helm

   
# Usage
## Login to k8s cluster
```yaml
- uses: freenet-actions/prepare-k8s-env@v1
  with:
    # in this case the secrets previously must be set bevor workflow run
    k8s-host-url: ${{ secrets.MY_K8S_HOST_URL }}
    k8s-token: ${{ secrets.MY_K8S_TOKEN }}
    k8s-cluster-name: ${{ secrets.MY_K8S_CLUSTER_NAME }} #optional
    k8s-user-name: ${{ secrets.MY_K8S_USER_NAME }} #optional
    kubectl-version: latest #optional, default: latest
    helm-version: 3.10.3 #optional, default: 3.10.3
```
