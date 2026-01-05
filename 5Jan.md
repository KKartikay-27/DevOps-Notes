# 5th January

[Notes](https://scaler-production-new.s3.ap-southeast-1.amazonaws.com/attachments/attachments/000/384/760/original/CompleteCITutorial__GitHub_Actions_DevSecOps_Pipeline__Java___Docker_.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIDNNIRGHAQUQRWYA%2F20260106%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20260106T112526Z&X-Amz-Expires=561600&X-Amz-SignedHeaders=host&X-Amz-Signature=44d4f7149585a0a2037cd0b881ddc52adc497d00dad900caaf13238e03c9e7bc)


## CI 

Github -> Linting -> Dependency -> SCA -> SAST -> Package -> Unit Testing ->  Docker Image Creation -> Testing images and containers -> Torque Scan -> Push to artifact repo 

**SCA - Software Compliance Analysis**

**SAST - Static Application Security Testing**


## Docker Integration
### Docker Setup
- Dockerfile kept with project code
- Docker handles containerization separately from Java

---

### Docker Hub
- Used to store Docker images
- Images built and pushed via GitHub Actions

---

## Secrets Management
- Never hardcode credentials
- Store sensitive data in:
  - GitHub Secrets
- Used for:
  - Docker Hub username
  - Docker Hub password / token

---

## Docker in GitHub Actions
- Automate:
  - Image build
  - Image push
- Use proper tags while pushing images

## Advanced CI Topics
- **Security Scanning**
  - Scan Docker images using Trivy
- **Static Analysis**
  - Tools like Checkstyle, CodeQL
- Helps maintain code quality and security
