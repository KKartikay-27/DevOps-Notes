# 14th Novemeber

[Notes](https://scaler-production-new.s3.ap-southeast-1.amazonaws.com/attachments/attachments/000/371/368/original/DockerContainers.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIDNNIRGHAQUQRWYA%2F20251117%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20251117T074417Z&X-Amz-Expires=561600&X-Amz-SignedHeaders=host&X-Amz-Signature=2676e599f607131ace42b576cb1b567acd1ebb35df4f343bca569cf4471ec852)

### How to differentiate between two VMs ?

1. Different Network stack
    - Port ranges
    - IP addresses
    - Socket ranges
2. Process Space
3. File System
4. Hostname space
5. User space
6. IPC - Inter Process Communication Call


*RPC - Remote Process Call*

**Two processes cannot run on the same port** 
eg. Tomcat and Nginx won't work together in the same port.

------

### docker run -d -p 80:80 nginx

**docker run**	- Start a new container

**-d**		- Run it in background

**-p 80:80**	- Map host port 80 → container port 80

**nginx**	    - Use the nginx image

---- 

## Docker Container 
Isolated environment but just a simple lightweight process in 
the host machine.


**Docker containers are ephemeral**

Meaning that they are designed to be thrown away and rebuilt when needed. This is useful for applications that are frequently updated or redeployed.


## C Groups / Control Groups 

C groups are a Linux kernel feature that allows you to limit, account for, and isolate the resource usage (CPU, memory, disk I/O, network, etc.) of a collection of processes. 

**C groups are used by Docker to limit the resources available to a container.**
