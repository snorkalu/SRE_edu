# SRE_edu


- [ ] Write ansible playbook to deploy postrgres using patroni setup
- [ ] Deploy etcd, patroni, postgres and Haproxy balancer insance
- [ ] Develop helm chart for deployment of api to k8s

```mermaid
deployment scheme:
    A[balancer]-->B[postgres_1];
    A[balancer]-->C[postgres_2];
    B[postgres_1]-->D[patroni_1];
    C[postgres_2]-->E[patroni_2];
    D[patroni_1]-->E[patroni_2];
```