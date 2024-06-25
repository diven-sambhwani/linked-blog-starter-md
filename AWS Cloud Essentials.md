
## Getting Started
Three key benefits of using cloud computing:
1. Programmable resources
2. Dynamic abilities
3. Pay as you go

Core service areas:
1. Compute
2. Storage
3. Databases
4. Networking
5. Security
![[Pasted image 20240225175953.png]]
## Understanding the AWS Global Infrastructure

![[Screenshot 2024-02-25 at 6.20.38 PM.png]]
1 Region has 2 or more Availability Zones, and 1 Availability Zone has 2 or more Data center, and 1 Data center has thousands of servers. This is where hardware is located.

## Core Services
### Compute
 EC2 -  Elastic Compute Cloud, provides scalable computing capacity in AWS. Amazon EC2 is a virtual machine launched on AWS hardware. 
 
 With Amazon EC2, you can add or remove EC2 instances and unhealthy applications _automatically_ and replace the instances _without_ intervention.

You can scale horizontally to precisely match the current demand and avoid overprovisioning or underprovisioning.

Amazon EC2 _does_ maintain and scale the fleet of nodes running your containers

 Different types mentioned below:
	- Virtual machines
	- Containers
	- Batch processing compute resources
	- Serverless compute
##### Instance Types
###### **Memory optimized**  
	When the most critical resource is RAM (memory), you will choose instances from within this family.
	**Examples of the Instance types:** r4, r5, x1, z1
	**Use case:** High compute and memory-intensive workloads

###### **Accelerated computing**
	when the focus is on the graphics processing unit (GPU).
	****Examples of the** Instance** **types:** f1, g3, g4, p2, p3
	**Use case:** Machine learning and high performance computing

###### **Storage optimized**
	when focusing on maximizing the number of **transactions per second (TPS)**
	****Examples of the** Instance types:** d2, h1, i3
	**Use case:** Maximize the number of transactions processed per second (TPS)

###### **General purpose**
	balance of compute, memory and networking resources
	****Examples of the** Instance types:** a1, m4, m5, t2, t3
	**Use case:** High performance file systems

######  **Compute optimized**
	ideal for compute bound applications that benefit from high performance processors.
	****Examples of the** Instance types:** c4, c5
	**Use case:** Network intensive workloads

###### **HPC optimized**
	**ideal for applications that benefit from high-performance processors** such as large, complex simulations and deep learning overloads.
	****Examples of the** Instance types:** Hpc6a, Hpc6id
	**Use case:** Best price performance for running HPC workloads
#####  Auto Scaling

**Amazon EC2 Auto Scaling helps maintain application availability and more.**

Auto Scaling helps you maintain application availability and automatically add or remove EC2 instances using scaling policies that you define.
Dynamic or predictive scaling policies let you add or remove EC2 instance in real-time 

Options:  manual, scheduled, dynamic or on demand, and predictive

##### Serverless

**building and running applications and services without managing servers.**

AWS Lambda is a fully managed serverless compute service.

- It is a great solution to be used in event-driven architectures.
- Provisioning, scaling, and underlying resources are taken care of by Lambda itself. 
- It provides high availability.
- Lambda offers per-millisecond pricing of the code being run.
-  Lambda can run your code in response to events or on a schedule 

##### Containers
Amazon Elastic Container Service (Amazon ECS) and Amazon Elastic Kubernetes Service (Amazon EKS) are the **container** **orchestrating services** that help you schedule, maintain, and scale the fleet of nodes running your containers.

**Amazon ECS**

Amazon ECS is an AWS container orchestration tool giving you seamless control over your containerized application.

**Amazon EKS**

Amazon EKS is a managed service that you can use to run Kubernetes on AWS without needing to install, operate, and maintain your own Kubernetes control plane or nodes. Kubernetes is an open-source system for automating the deployment, scaling, and management of containerized applications.

Amazon ECS and Amazon EKS give you a _centralized_ way of monitoring and controlling how you want your containers launched.

f you have in-house skills running Kubernetes, _there is a fully managed_ Amazon EKS for you.

Amazon ECS and Amazon EKS are container orchestrating services that _help you schedule_ the fleet of nodes running your containers.

Amazon ECS and Amazon EKS _remove_ the complexity of standing up the infrastructure.

### Storage
