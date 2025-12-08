# 8th December

[Notes](https://scaler-production-new.s3.ap-southeast-1.amazonaws.com/attachments/attachments/000/377/019/original/006_Kubernetes_Services.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIDNNIRGHAQUQRWYA%2F20251215%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20251215T081227Z&X-Amz-Expires=561600&X-Amz-SignedHeaders=host&X-Amz-Signature=5e007fa7c8c794576250350d515559215df88fcb6912877d3da437f8748d39fc)

### Pods 
- Pod represents a running process in the cluster
- Pods:
  - Share IP address
  - Share port space

## ReplicaSets
- Maintains a fixed number of pod replicas
- Automatically recreates pods on failure
- Even single-pod apps benefit from ReplicaSets for recovery

## Deployments
- Declarative way to manage ReplicaSets and Pods
- Handles:
  - Scaling
  - Rolling updates
  - Rollbacks
- Internally manages ReplicaSets

## Services
- Provide a stable network endpoint for pods
- Uses labels to route traffic to correct pods

### Types of Services
- **ClusterIP**
  - Accessible only within the cluster
- **NodePort**
  - Exposes service on each node’s IP and port
  - Automatically creates a ClusterIP


## Service Concepts
- **Service Discovery**
  - Services find pods using labels
- **Load Balancing**
  - Traffic distributed evenly across pods


## Load Balancers
- Used to distribute traffic across pods
- **Internal LB**
  - Used within the cluster
- **External LB**
  - Handles incoming internet traffic
