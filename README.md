# Welcome overview
Hello dudes,  
This is my main share for All SRE tools i know and modified for run in my private environments.  
In all my documents, i will show you guys how to build those tools quickly before explain how it works, just 5 minutes required every topic  
My vision is after all bellow topics, you can install all requirement applications for SRE and also provide it with Gitops(basic) to team working in your corporate  
After all you will get experience for all monitoring tool as bellow diagram
![alt text](https://github.com/JemieLoopy/sre-automation-sharing/blob/main/global-imgs/sre-tools.png?raw=true)

### Note  
So you must install all requirement tools  to avoid any exception issues
Hope it help some new guys 
I will update one by one every weekend or if you guys need help, please sent email to me: jemieloopy@gmail.com

### How to
Requirement Tools:
 - Client Tools in your PC: kubectl, helm, helmfile, helmdiff plugin, git. [view guide](https://github.com/JemieLoopy/sre-automation-sharing/tree/main/requirement-tools)
 - K8S Cluster with: ingress nginx, metal-lb, storage-class
 - Provision Minio Distributed(s3 storage require for some important backend to run in Large Production env). [view guide](https://github.com/JemieLoopy/sre-automation-sharing/tree/main/minio-distributed)
 - Provision Harbor Private registry(I don't want to get every thing from internet cause some security reasons). [view guide](https://github.com/JemieLoopy/sre-automation-sharing/tree/main/private-registry)

Monitoring Tools:
 - Provision Prometheus for monitor k8s cluster and services (Gitops)
 - Provision Grafana OSS (Mimir metrics,Loki Loggings,Tempo Tracing) for long time and scalable store
 - Provision ELK stack
 - Provision Grafana with Terraform
 - Grafana Oncall

SRE Alert:
 - Provision prometheus-alertmanager alert with Gitops
 - Provision metrics(Mimir) alert in Grafana Oncall with Gitops
 - Provision logging(Loki) alert in Grafana Oncall with Gitops
 - Provision Elasticsearch alert in Grafana Oncall with Gitops

SLI, SLO builder:
  - Updating

SRE dashboard:
  - Provision Grafana Dashboard with Gitops
  - Provision Kibana Dashboard with Gitops  

SRE Report:
 - Provision Grafana PDF Exporter -> Export Grafana Dashboard as pdf and sent email
 - SLO,SLI Reports

