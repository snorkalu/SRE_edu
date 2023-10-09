# SRE_edu


- [X] Write ansible playbook to deploy postrgres using patroni setup
- [X] Deploy etcd, patroni, postgres and Haproxy balancer insance
- [X] Develop helm chart for deployment of api to k8s
- [X] Create DB using script from api docker, add records

Deployment scheme
[![Alt text]([https://static.tildacdn.com/tild3835-6161-4534-a135-323838653733/image.png)]

Ansible playbook


```ansible-playbook -i inventory deploy_pgcluster.yml```


helm
helm install api-student78 api-student78 
