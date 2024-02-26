# Minio Distributed S3 storage
## Prepare:
Visit homepage: https://github.com/minio/minio/tree/master/helm/minio
**Prepare your helmfile**  
Create file: helmfile.yaml 
```
repositories:
- name: minio
  url: https://charts.min.io/
releases:
- name: minio-distributed
  namespace: your_namespace
  values:
  - ./minio-distributed-values.yaml
  chart: minio/minio
  version: 5.0.13
```
**Prepare your minio config**  
Create file: minio-distributed-values.yaml with your own content,  
See  [example](https://github.com/JemieLoopy/sre-automation-sharing/tree/main/minio-distributed/minio-distributed-values.yaml)  
In this example, i create 1 pool with 3 replicas and persistent volume 100GB  


## Install:
Run command to add repo:  
```
cd minio-distributed
helmfile repos
helmfile apply --selector name=minio
# You can run simply: helmfile sync

```
