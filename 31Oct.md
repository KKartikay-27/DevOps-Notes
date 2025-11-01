# 31st October

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