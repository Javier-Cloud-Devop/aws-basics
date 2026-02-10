# Highly Available Web Applications
---

## Description
This lab focuses on deploying a highly available web application across multiple Availability Zones using an Application Load Balancer and an Auto Scaling group

---

## Scenario
A web application must remain available even if an Availability Zone or EC2 instance fails
Traffic should be distribuited across multiple instances, and unhealthy instances must be automatically replaced
The architecture must support high availability and fault tolerance

## Key concepts explored
- Multi-AZ architecture
- Aplication Load Balancer (ALB)
- Auto Scaling Group integrated with ALB
- Health Checks
- High availability design
- Basic fault tolerance

---

## Observations
- The Applicacion Load Balancer distributes traffic across EC2 instances in different Availability Zones
- Helath checks allow the Auto Scaling Group to detect and replace unhealthy instances automatically
- Adding additional Availability Zones improces reilience without changing application logic
- Auto Scaling Groups and load balancers work together to provide both availability and scalability

---

## Tool used
- AWS Management Console (GUI)
- Amazon EC2
- EC2 Auto Scaling
- Elastic Load Balancing (Applicacion Load Balancer)
- Target Groups
