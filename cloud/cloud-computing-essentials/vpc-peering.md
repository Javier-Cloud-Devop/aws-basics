# Connecting VPCs using Peering

## Description
- This lab focused on enabling communication between multiple Amazon VPCs peering connection

- The scenerio involved three separate VPCs representing different departments:
  - Marketing
  - Finance
  - Development

## Initial state
- Each VPC was isolated
- EC2 instances could not communicate using private IP addresses
- Connectivity was tested using ping via AWS Systems Manager Session Manager

## Steps performed
- Created a VPC peering connection between Marketing and Finance
- Accepted the peering connection from the Finance VPC
- Updated route tables in both VPCs to route traffic to the peered CIDR blocks
- Verified that connectivity was still blocked due to security restrictions
- Updated  Security Group rules to allow inbound traffic from the peered VPC CID ranges

## Key concepts learned
- VPCs are isolated by default in AWS
- VPC peering requires configuration on both sides
- Route tables control traffic flow but do not grant permission
- Security Groups must explocitly allow traffic between peered VPCs
- Network connectivity in AWS requires routing and security alignment

## Tool used
- AWS Management Console (GUI)
- Amazon VPC
- VPC Peering
- Route tables
- Security Group
- AWS Systems Manager Session Manager
  
