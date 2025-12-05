# 5th December

[Notes](https://scaler-production-new.s3.ap-southeast-1.amazonaws.com/attachments/attachments/000/376/201/original/005_Kubernetes_Deployment.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIDNNIRGHAQUQRWYA%2F20251208%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20251208T080434Z&X-Amz-Expires=561600&X-Amz-SignedHeaders=host&X-Amz-Signature=1118935777d3fb29988be1b64708a3a84a6ff730ee64091eb9889e27e41cedf7)


## ReplicaSets
- Ensures a fixed number of pod replicas
- Handles pod or node failures automatically
- Used mainly by Deployments, not directly in production

## Deployments
- Manages:
  - Pod creation
  - Updates
  - Scaling
  - Rollbacks


## Scaling & Rollouts
### Scaling
- Replica count can be increased or decreased
- Can be done using `kubectl scale`

### Rolling Updates
- Default strategy for deployments
- Updates pods gradually
- No downtime during updates

---

## Upgrade & Rollback
- Deployments keep revision history
- Easy to rollback to a previous version
- Useful in CI/CD pipelines


## Best Practices
- Prefer YAML over imperative commands
- Store configs in version control
- Use namespaces for environment separation
- Monitor desired vs actual state
