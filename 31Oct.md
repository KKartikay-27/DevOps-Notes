# 31st October

[Notes](https://scaler-production-new.s3.ap-southeast-1.amazonaws.com/attachments/attachments/000/368/649/original/003AWSAndLinuxIntroduction.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIDNNIRGHAQUQRWYA%2F20251103%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20251103T074810Z&X-Amz-Expires=561600&X-Amz-SignedHeaders=host&X-Amz-Signature=a4855f13c7801e59fb758b459283d558d26670db0b7fc38d0ddc763d840a03da)

## CI Revision
Fork repo -> Download Code -> Linting -> Build -> Unit Test -> SCA -> SAST -> Dockerize (Create docker images) -> Dynamic Testing -> Push image into Artifact repository 

**SCA - Software Compliance Analysis**

**SAST - Static Application Security Testing**

## CD (Continuous Deployment/Development/Delivery)

**SIT - System Integration Testing**

Artifactory (Artifact Repository) -> SIT -> Performance Testing -> Security Testing -> DAST -> Production Deployment

**DAST - Dynamic Application Security Testing** 

*SIT -> Deployed and Automated Testing
                                    
Artifact examples -
- Zip
- JAR/WAR
- gems
- .exe/ISO
- Docker images

### Line Coverage
    is a software testing metric that measures the percentage of executable lines of code that are run by a test suite.

### Function Coverage
    is a testing metric that measures which functions in a program have been called during a test run.

### Code coverage
    is a metric in software testing that measures the percentage of source code executed by a test suite, helping developers identify untested parts of an application.

# In project, write code for DAST

## Linux Referesher

### Unix 
Popular in 1969 -> 1990

### Kernel  
- Interface between hardware
- Manage
    - CPU
    - Memory
    - Hard Disk (H/D)

### Micro Kernel Architecture (----)
is a design approach that keeps the core operating system functions minimal, handling only the most essential tasks like memory management, process scheduling, and inter-process communication. 

### VPC 
Virtual Private Cloud in a region

IP Address
- Public IP -> Anybody
- Private IP -> Only within AWS
- Elastic IP -> Can be attached to a Public IP. It remains stable even if the instance is restarted or moved to a different region.