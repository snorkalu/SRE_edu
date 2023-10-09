# SRE_edu


- [X] Write ansible playbook to deploy postrgres using patroni setup
- [X] Deploy etcd, patroni, postgres and Haproxy balancer insance
- [X] Develop helm chart for deployment of api to k8s
- [X] Create DB using script from api docker, add records

Deployment scheme
[![Scheme]([https://static.tildacdn.com/tild3835-6161-4534-a135-323838653733/image.png])]

**Ansible playbook**

based on https://github.com/vitabaks/postgresql_cluster

all host are described in inventory

run from host having access to hosts.

useful commands:

deploy
```ansible-playbook -i inventory deploy_pgcluster.yml```
reset pg cluster config
```ansible-playbook -i inventory config_pgcluster.yml```

**helm**

run from host with kubectl 
useful commands:
```helm install api-student78 api-student78```
```helm upgrade api-student78 api-student78```
