### Overview
This repo includes manifests for setting up experiment environment.  
The following resources will be created after setup.
- prometheus-operator and all the CRDs managed by it
- basic RBAC settings for prometheus-operator and prometheus
- all the resources shown in the high level diagram
- an additional prometheusRule-backend resource
#### Note
This repo is not mean to be used for bootstrapping monitoring stack.  
Therefore, the lack of some critical components is as expected.
### Environment Setup
```
git clone https://github.com/wlog106/xuanhh-sysnewbie-report.git
cd xuanhh-sysnewbie-report
kubectl create -f manifests/setup -R
kubectl create -f manifests/prometheus-operator
kubectl create -f manifests/
```
### Reference
- [prometheus-operator official website](https://prometheus-operator.dev/)
- [prometheus-operator github page](https://github.com/prometheus-operator/prometheus-operator)
- [kube-prometheus github page](https://github.com/prometheus-operator/kube-prometheus)
