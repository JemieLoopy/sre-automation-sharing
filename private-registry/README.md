# Minio Distributed S3 storage
## Prepare:
**Prepare your helmfile**  
Create file: helmfile.yaml 
```
repositories:
- name: harbor
  url: https://helm.goharbor.io
releases:
- name: harbor
  namespace: your_namespace
  values:
  - ./harbor-values.yaml
  chart: harbor/harbor
  version: 1.11.0
```
**Prepare your minio config**  
Step 1: you need to create minio s3 bucket to save long time and big data   
Step2: Create file: harbor-values.yaml with your own content and don't forget to input s3 bucket as backend storage,    
See  [example](https://github.com/JemieLoopy/sre-automation-sharing/tree/main/private-registry/harbor-values.yaml)  


## Install:
Run command to add repo:  
```
cd private-registry
helmfile repos #this command add repo with helmfile
helmfile apply --selector name=harbor
# You can run simply: helmfile sync

```
