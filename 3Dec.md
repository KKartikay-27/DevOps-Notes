# 3rd December

[Notes](https://scaler-production-new.s3.ap-southeast-1.amazonaws.com/attachments/attachments/000/375/417/original/003ReplicaSet___Deep_Technical_Tutorial.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIDNNIRGHAQUQRWYA%2F20251208%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20251208T080437Z&X-Amz-Expires=561600&X-Amz-SignedHeaders=host&X-Amz-Signature=3de33b504b596d5dbc31c6ee8336c6554373c94176e725fe12594bcc9c4852cd)



### Kubernetes 
## Pods
- Smallest deployable unit in Kubernetes
- Can contain one or more containers
- Containers in a pod:
  - Share network and storage
  - Are scheduled on the same node
- If a container crashes, Kubernetes recreates it automatically



## ReplicaSets
- Ensures a fixed number of pod replicas are always running
- If a pod or node fails, new pods are created automatically

**Kubelet** – Manages pods on a node

**Scheduler** – Assigns pods to nodes


kubectl apply -f file.yaml

kubectl delete -f file.yaml

kubectl get pods
