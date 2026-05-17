### Overview
This repo include manifests for setting up experiment environment.  
The following resources will be created after setup.
- prometheus-operator and all the CRDs managed by it
- basic RBAC settings for prometheus-operator and prometheus
- All the resources shown in experiment environment graph
#### Note
This repo is not mean to be used for bootstrapping monitoring stack.  
Therefore, the lack of some critical components is expected.
### Environment Setup
```
kubectl create -f manifests/setup -R
kubectl create -f manifests/prometheus-operator
kubectl create -f manifests/
```
### Reference
- RBAC: [prometheus-operator official docs](https://prometheus-operator.dev/docs/platform/rbac/)
- CRDs: [kube-prometheus quick start manifests](https://github.com/prometheus-operator/kube-prometheus/tree/main/manifests/setup)
