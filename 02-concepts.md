## Vocabulary in Cloud Computing

## Virtulization

In simple terms Virtulization is the process of creating a virtual version of something such as an operating system, server, storage or network resources.

Virtualization is the technology that allows multiple virtual resources (servers, storage, networks, operating systems) to run on a single physical machine.

It works using a hypervisor which divides the physical hardware into multiple virtual environments.

Example technologies:
- VMware ESXi
- KVM
- Microsoft Hyper-V

- Why it matters in cloud:
Cloud providers like Amazon Web Services rely heavily on virtualization to create thousands of virtual servers from physical hardware.

## Virtual Machine

A Virtual-Machine (VM) is a software-based emulation of a physical computer. It allows running multiple operating systems on a single physical machine.

A Virtual Machine (VM) is a software-based computer that runs an operating system and applications just like a physical computer.

Multiple VMs can run on one physical server.

Example:
You can run:
Linux VM
Windows VM
on the same physical machine.

Example cloud service:
Amazon EC2 provides virtual machines in the cloud.

## API (Application Programning Interface)

API is a set of rules and protocol that allows a different software applications to communicate each other. It define how software components should interact.

An API is a set of rules that allows different software applications to communicate with each other.

It defines how requests and responses should be structured.

Example:
When you create a server in
Amazon Web Services, your command or console action actually calls an AWS API behind the scenes.

Example tools that interact with APIs:
- Postman
- cURL

## Regions

Regions in cloud computing refers to geograpic locations where cloud providers have data centers. Each region contains multiple data centers.

A Region is a geographical area where a cloud provider operates multiple data centers.

Example regions in Amazon Web Services:
- US East
- Europe 
- Asia Pacific

Regions help with:
- low latency
- regulatory compliance
- disaster recovery


## Availability Zones

Availability Zones are isolated locations within a region that have their own power, cooling and networking. They are designed to provide high availability and fault tolarance.

An Availability Zone is an isolated data center within a region.

Each AZ has:
- independent power
- independent network
- independent cooling

This design helps achieve high availability.

Example:
AWS Mumbai Region:
- AZ-1
- AZ-2
- AZ-3

Applications can run across multiple AZs to avoid downtime.

## Scalability

Scalability is the ability of a system to handle increasing workloads by adding resources.

Two types:
- Vertical Scaling
Increase power of a single machine.
Example:
4 CPU → 8 CPU
16GB RAM → 32GB RAM

- Horizontal Scaling
Add more servers.
Example:
1 server → 10 servers.
Horizontal scaling is more common in cloud systems.

## Elasticity

Elasticity is the ability to automatically increase or decrease resources based on demand.

Example:
During a big sale:
- traffic increases
- servers automatically increase
After the sale:
- extra servers automatically stop.

Example service:
- Amazon EC2 Auto Scaling

## Agility

Agility is the capability of quickly and easily adapting to changes. In the context of cloud computing , it involves the rapid deployment of resources and applications.
Agility in cloud computing means the ability to rapidly deploy and configure resources.

Instead of waiting weeks for hardware:

You can create a server in minutes using
Amazon Web Services.

## High Availability

High Availability ensures that systems remain operational for a very high percentage of time.

Typical uptime targets:
99.9% → ~8 hours downtime/year
99.99% → ~52 minutes downtime/year

HA is achieved using:
multiple servers
multiple availability zones
load balancing

## Fault Tolerance

Fault Tolerance is the ability of a system to continue operating even if one or more components fail.

Example:
If one server crashes:
    - another server immediately takes over.
Fault tolerance often uses redundant infrastructure.

## Disaster Recovery

Disaster Recovery (DR) is the planning and processes for restoring and recovering data and systems after a natural or human-induced disaster.

Disaster Recovery is a strategy to restore systems and data after major failures such as:
    earthquakes
    power outages
    cyber attacks
    data center failures

- Common DR methods:
    data backups
    cross-region replication
    failover systems

Example:
Replication between two regions in
Amazon Web Services.

## Load Balancing

Load Balancing distributes incoming traffic across multiple servers to prevent any single server from becoming overloaded.

Benefits:
improved performance
high availability
fault tolerance

Example service:
AWS Elastic Load Balancer