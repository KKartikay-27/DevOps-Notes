# 1st December

[Notes](https://scaler-production-new.s3.ap-southeast-1.amazonaws.com/attachments/attachments/000/375/416/original/002PodDeepDive.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIDNNIRGHAQUQRWYA%2F20251208%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20251208T080442Z&X-Amz-Expires=561600&X-Amz-SignedHeaders=host&X-Amz-Signature=f3de87788923563980cd9e7f11ee31f9aaa8dbde58b5bb214918e6fa57e1c3e3)

## Kubernetes – Basics & Architecture

### Cluster Setup
- Kubernetes cluster was shown using **3 machines**
  - 1 Master node
  - 2 Worker nodes
- Master controls the cluster
- Workers run the actual applications

---

## Master Node
- Instructor had already done some initial setup
- Used shell script for installation
- Master initialized using:
  - `sudo su`
  - `kubeadm init`
- This sets up:
  - API Server
  - etcd
  - Controller
  - Scheduler

---

## Pods
### What is a Pod?
- Smallest unit in Kubernetes
- Can have **one or more containers**

### Pod Characteristics
- Network
- Storage

---

## Kubernetes Architecture

### Control Plane
- API Server
- etcd (stores cluster state)
- Controller
- Scheduler

### Data Plane
- Runs workloads on worker nodes
- Handles actual application execution


## Working with Pods
- Pods created using `kubectl`
- `kubectl get pods`

## Namespaces
- Used to organize and isolate resources
- Default namespaces:
  - `default`
  - `kube-system`

