# 24th November

## Kubernetes

- Orchestrate containers
- Automatic bin packing
- Fail over
- Automatic scaling
- Load balancing
- Service discovery
- Jobs
- Secrets
---
Kubernetes is an open-source container orchestration platform that automates the deployment, scaling, and management of containerized applications. 

It provides a way to manage and run containerized applications at scale, with features such as self-healing, load balancing, and service discovery.

---

## Kubernetes Architecture

Two type of machines -
- Control Plane / Master Node
- Data plane / Work Node

Node - Virtual Machine or Physical Machine

API servers
- Authentication
- Authorization
- Validation
- Talk to ETCD

**ETCD is an open-source, distributed, consistent key-value store used as the primary data store for distributed systems like Kubernetes.**

### Scheduler -
A scheduler is a component of Kubernetes that assigns pending pods to nodes in the cluster.
