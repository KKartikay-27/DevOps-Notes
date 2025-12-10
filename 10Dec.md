# 10th December

[Notes](https://scaler-production-new.s3.ap-southeast-1.amazonaws.com/attachments/attachments/000/377/256/original/007_Kubernetes_Networking_Model_Deep_Dive.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIDNNIRGHAQUQRWYA%2F20251215%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20251215T081122Z&X-Amz-Expires=561600&X-Amz-SignedHeaders=host&X-Amz-Signature=78b8bbbbc6a5fb468b34df632053498858c83b1e003b1be1e11ccc922928ec45)


### Pod Networking (Same Pod)
- A pod acts as a single network unit
- Containers inside a pod:
  - Share the same network namespace
  - Communicate using `localhost`
- Works like multiple processes running on one machine

## Pod-to-Pod (Same Node)
- Pods on the same node communicate via a virtual network
- Managed by CNI (Container Network Interface) plugins
- Network plugin handles IP allocation and routing


## Pod-to-Pod (Different Nodes)
- Communication across nodes handled using:
  - Network plugins
  - IP tables
- Traffic is routed based on rules set on each node

### kube-proxy
- Maintains networking rules on nodes
- Updates IP tables
- Helps route traffic to correct pods


## Pod-to-Service Communication
- Services provide a stable endpoint for pods
- Each service gets a **ClusterIP**
- Traffic is load-balanced across matching pods

## Service Discovery
- CoreDNS maps service names to IP addresses
- Pods can access services using names instead of IPs
- Service endpoints updated dynamically
