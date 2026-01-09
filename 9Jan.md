# 9th January

## Terraform & Infrastructure as Code (IaC)

### What is Terraform
- Open-source IaC tool
- Manages cloud infra using code
- Works across providers (AWS, Azure, GCP)
- Platform agnostic

## Why Infrastructure as Code
- Eliminates manual setup errors
- Ensures repeatability and consistency
- Easy rollback using version control

## Terraform Lifecycle Commands

### terraform init
- Initializes working directory
- Downloads required providers & modules
- Locks provider versions

### terraform plan
- Compares current vs desired state
- Shows execution plan
- No actual changes applied

### terraform apply
- Applies planned changes
- Creates/updates infrastructure

### terraform destroy
- Deletes all managed infrastructure
- Cleans up resources completely

## Advantages of Terraform
- Faster infra provisioning
- Consistent environments
- Git-based version control
- Easy auditing and rollback

## Related Tools

### Configuration Management
- Ansible
- Puppet
- Chef

(Used for software/config after infra creation)

### Server & Environment Tools
- Vagrant
- Docker

(Used for VM and container environments)

