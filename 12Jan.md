# 12th January

### Subnets
- Subnet = range of IPs inside a VPC
- Two types:
  - **Public subnet** → connected to Internet Gateway
  - **Private subnet** → no direct internet access


## Terraform Dependencies
- Terraform figures out resource order automatically
- If one resource references another, dependency is implicit
- No need to manually define order in most cases

## VPC & Networking

### VPC
- Virtual network inside AWS
- Isolated per AWS account

### CIDR Block
- Defines IP range for VPC
- Controls size of network

### Route Tables
- Decide where traffic goes
- Based on destination IP

## Terraform State
- Terraform uses `terraform.tfstate`
- Tracks real infra vs config
- For teams:
  - Use **remote state**
  - S3 for state storage
  - DynamoDB for state locking

## Terraform File Structure
Common files:
- `main.tf` → main config
- `network.tf` → VPC, subnets, gateways
- `compute.tf` → EC2, security groups

Names aren’t mandatory, just convention.

## Types of IPs
- **Private IP** → internal VPC communication
- **Public IP** → internet access
- **Elastic IP** → static public IP, reusable

## EC2 Basics
- AMI is mandatory to launch EC2
- AMI defines OS and base setup


## Variables in Terraform
- Input variables → configurable values
- Output variables → show useful info
- Local variables → limited scope
