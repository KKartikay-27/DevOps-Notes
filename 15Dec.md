# 15th December

[Notes](https://scaler-production-new.s3.ap-southeast-1.amazonaws.com/attachments/attachments/000/378/676/original/HPA.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIDNNIRGHAQUQRWYA%2F20260203%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20260203T173557Z&X-Amz-Expires=561600&X-Amz-SignedHeaders=host&X-Amz-Signature=9bd072051e5fd88524bcab3dc96671bb80853730cb7001bd4c0274b02370233d)

### Horizontal Pod Autoscaler (HPA)

- HPA automatically adjusts the number of pod replicas
- Scaling is based on:
  - CPU utilization
  - Memory or custom metrics
- Works with:
  - Deployments
  - ReplicaSets
  - StatefulSets


## Horizontal Scaling
- Scaling happens by **adding or removing pods**
- When load increases → more pods
- When load decreases → fewer pods

## Prerequisites for HPA
- Kubernetes cluster
- Metrics Server must be running
  - Required for CPU and memory metrics


## Core Components Involved
- **kubeadm** – Initializes the cluster
- **kubectl** – Used to manage cluster resources
- **kubelet** – Runs on each node and reports metrics

## Metrics Server
- Collects CPU and memory usage
- Exposes metrics via Kubernetes API
- Without it, HPA will not work

