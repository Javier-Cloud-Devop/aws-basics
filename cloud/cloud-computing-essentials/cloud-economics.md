# Cloud Economics - EC2 Cost Estimation

## Description
This lab focused on understanding AWS cloud costs by creating a pricing estimate using the AWS Pricing Calculator

The goal was to estimate the cost of an EC2-based architecture with variable demand and analyze how pricing models affect overall cost

## Scenario 
- Baseline workload:
  - 2 x EC2 te.small instances running continuosly
- Peak workload:
  - Up to 2 additional EC2 instances
  - Peak usage assumed for 8 hours per day
- Storage:
  - Amazon EBS volumes
  - Weakly snapshot for backup
 - Data transfer:
   - Inbound and outbound traffic considered
  
## Key concepts explored
  - On-Demand vs REserved Instances (1-year commitment)
  - EBS impact of scaling during peak demand
  - EBS volume and snapshot pricing
  - Data tranfer costs (indboutn vs outbound)
  - AWS Support plans (Basic to Enterprise)

## Observations
- On-Demand pricing offers flexibility but is significantly more exensive than long-term
- Reserved Instances reduce costs considerably for precistable workloads
- Storage and data transfer costs must be included in rel estimates
- AWS Support plans can become a significant cost for businesses
- Static websites are usually more cost-efficient when hosted on Amazon S3 instead of EC2

## Tools used
 - AWS Pricing Calculator
