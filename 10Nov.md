# 10th November

[Notes](https://scaler-production-new.s3.ap-southeast-1.amazonaws.com/attachments/attachments/000/370/465/original/DockerIntroAndImages.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIDNNIRGHAQUQRWYA%2F20251112%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Date=20251112T075021Z&X-Amz-Expires=561600&X-Amz-SignedHeaders=host&X-Amz-Signature=f59ca6d834f188b48a8afafbc2410c307630b64995c18f356ee8103b9b953f48)

### Docker always relies on the kernel of the host operating system, regardless of which OS you’re using.

Here’s the key point:

- Containers share the host’s kernel, unlike virtual machines which have their own separate kernel inside a guest OS.

- That means if you’re running Docker on Linux, containers directly use the Linux kernel features like cgroups, namespaces, and union file systems.

- If you’re running Docker on Windows or macOS, Docker actually runs a lightweight Linux virtual machine in the background (using WSL2 on Windows, or a LinuxKit VM on macOS), because containers need Linux kernel functionality.

## Hypervisor
A hypervisor is a special layer of software (or firmware) that allows multiple virtual machines (VMs) to run on a single physical computer by sharing its hardware resources — CPU, memory, storage, and network — securely and efficiently.

It’s also called a Virtual Machine Monitor (VMM).

----

## Physical Machine
![alt text](images/PhysicalMachine.png)

lib - libraries

bin - binaries (Variables)

## Virtual Machine
![alt text](images/VirtualMachine.png)


**Hypervisor can help us to run multiple virtual machines on a single physical machine.**

![alt text](images/"Docker"Machine.png)

Docker helps in making containers on top of the virtual machine.

![alt text](images/Comp.png)


### BIOS - Basic Input Output System

BIOS, or Basic Input/Output System, is the firmware on a computer's motherboard that initializes and tests hardware during the boot process, then loads the operating system

    |
    V
### MBR - Master Boot Record 

MBR is most commonly an abbreviation for Master Boot Record, a critical data structure on a computer's hard drive that contains boot code and a partition table to start the operating system

    |
    V
### Boot Loader 

Boot Loader is a program that loads an operating system into memory from a storage device.

    |
    V
### Kernel 

Kernel is the core of the operating system, responsible for managing system resources and providing services to other software components.

    |
    V
### INIT

INIT is the first process that runs when the system starts up. It is responsible for starting other processes and services.

    |
    V

### Processes

    |
    V

### App

-----

### What happens when you execute the Docker run command -

![alt text](images/ContainerRunning.png)

## Docker Architecture

![alt text](images/DockerArch.png)

------
------
------
**Docker container is somewhat like a Lightweight Virtual Environment, not a Virtual Machine or Virtual Machine Monitor (VMM). And it's isolated from one another. It is generally more lightweight and efficient than VMs.**

**VMs are heavyweight and resource-intensive because they require a full-fledged operating system to run inside them. In contrast, Docker containers run directly on the host machine's kernel, sharing it with other containers. This makes them more resource-efficient and faster to start up.**

**Additionally, Docker containers are platform-independent, meaning they can run on any host machine that supports Docker, regardless of the underlying operating system. This makes it easier to deploy applications across different environments.**

**So, Docker containers offer many advantages over VMs, including lightweight resource usage, platform independence, and faster startup times.**

------
------
------

### docker container prune - Removes all the stopped containers