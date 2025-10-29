# 27th October

## Course Structure

- Microservices Architecture
- Devops Intro
- Linux Refresher
- Shell Scripting
- Git Refresher
- Docker
- Kubernetes
- Github
- Terraform

## Microservices Architecture

Searching on web browsers ask DNS servers to resolve the IP address of the website.

Search on browser -> DNS Server -> IP Address -> Web Server -> Response

A load balancer typically distributes the traffic to servers, but it can also redirect the traffic.

- Path based routing 
- Instance identification within a service

**Authorization vs Authentication**

(Modi - Chapraasi)
- Authentication - Verifying who you are
- Authorization - Verifying what you are allowed to do

In monolithic codebase, it interacted with a database. But single database + service cannot scale.

Microservice contact each other using APIs.

##### In microservices, different languages and frameworks can be used to build different services and they interact through APIs.

Most services to service calls would typically need a load balancer to distribute the traffic to multiple instances of the called service, but not always. Depending on the architecture, some services might not need a load balancer.

###  Synchronous calls vs Asynchronous calls

(Couple over call vs Couple over WhatsApp)

- Synchronous calls - The caller waits for the response from the called service.
- Asynchronous calls - The caller does not wait for the response from the called service.

For synchronous calls, need a message broker like Kafka and RabbitMQ, respectively.

**Asynchronous calls are generally considered better and faster.**

### Asynchronous Types -

1. Queue Model Architecture - Broker will carry the message.
2. Publish Subscribe Architecture (PubSub) - Publisher will publish the message, subscriber gets the message.

(No need of a load balancer)
1. Kafka is smart enough to replace a load balancer
2. No need of a load balancer, direct calls to service instances  

### Event Syncing 
Event Syncing is the process of maintaining the state of systems in near real-time by synchronizing the events that occur in those systems. Event syncing is also known as event seeking.


**12 Factor App - https://12factor.net/**

### Service Dependency and Component Dependency

**Service Dependency**
Microservices depend on each other and interact using APIs.




