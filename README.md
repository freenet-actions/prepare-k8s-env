# k8s-login-action
[![LICENSE](https://img.shields.io/github/license/freenet-actions/k8s-login-action)](https://github.com/freenet-actions/k8s-login-action/blob/main/LICENSE)

This action implements the Kubernetes (K8s) cluster registration.

   
# Usage
## Login to k8s cluster
```yaml
- uses: freenet-actions/k8s-login-action@v1
  with:
    # in this case the secrets previously must be set bevor workflow run
    k8s-host-url: ${{ secrets.MY_K8S_HOST_URL }}
    k8s-token: ${{ secrets.MY_K8S_TOKEN }}
    k8s-cluster-name: ${{ secrets.MY_K8S_CLUSTER_NAME }} #optional
    k8s-user-name: ${{ secrets.MY_K8S_USER_NAME }} #optional
```

## Requirements
The kubectl tool must be installed on GitHub runner.
