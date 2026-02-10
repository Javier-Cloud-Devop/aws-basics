# Auto-HEaling and Scaling Applications

---

## Description
This lab focused on configuring an EC2 Auto Scaling solution to automatically manage instance availability and capacity based on predefined schedules

---

## Scenario
A game applicacion runs on EC2 instances and expreiences predictable peaks in user traffic. 
The infrastructure must be able to:
- Autmoatically increase capacity duting high-demand periods
- Reduce or stop instances during los-demand periods to optimize costs
- Recover automatically bu launching new instances when required

---

## Key concepts explored

- EC2 Auto Scaling Groups
- Launch Templates
- Amazon Machine Images (AMI)
- Scheduled scaling actions
- Basic auto-healing concepts
- Cost optimization through scaling policies

---

## Observations

- Auto Scaling Group rely on Launch templates to define how instances are created
- Scheduled scaling is useful when traffic patterns are predictable and known in advance
- Scaling down to zero instances during off-hours significantly reduces costs
- This lab did not use load-based scaling policies; scaling decisions were time-based

---

## Tool used

- AWS Management Console (GUI)
- Amazon EC2
- EC2 Auto Scaling
- Amazon CloudWatch
- Amazon Machine Image (AMI)
