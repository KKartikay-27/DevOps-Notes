# 7th January

## CD

Artifactory (Pick up artifact / docker image, JAR, WAR) -> Deploy and Test into SIT (System Integration Testing) -> Performance Testing (Test and Deploy) -> Security Testing (Injection Test & SQL Injection test) -> NLP Integration and Testing (Optional)

- **Continuous Integration (CI)**
  - Frequent code merges
  - Automated builds and tests
  - Keeps codebase deployable
- **Continuous Deployment (CD)**
  - Automatically deploys changes
  - Focus on zero-downtime releases
  - Handles infra + app deployment


## Kubernetes Environment
- Kubernetes should be pre-installed on the VM
- Using pre-built images (AMI) saves setup time
- Cluster acts as the deployment target for CD

## GitHub Actions
- Used to automate CI/CD pipelines
- Handles:
  - Build
  - Test
  - Deploy
- Integrated directly with the GitHub repo

## Custom (Self-Hosted) Runners
- Alternative to GitHub-hosted runners
- Machine registers itself as a runner
- Commonly set up on Linux

### Runner Setup
- Register using `config.sh`
- Assign labels for job targeting
- Needs proper security configuration

## Project Work
- Team-based CI/CD project
- Each member responsible for their contribution
- Individual understanding checked during review

## Testing Strategy
- Multiple testing stages:
  - SIT
  - Performance testing
  - Security testing
- Tests are usually automated
