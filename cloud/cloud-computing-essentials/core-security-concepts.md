# Core Security Concepts (IAM)
---
## Description 
This lab focuses on implementing basic IAM security concepts using groups, users, and managed policies to enforce least-privilege access to AWS resources. 

---

## Scenario
Support engineers require controlled access to AWS resources
They must be able to view infrastructure resources without being allowed to modify or delete them
Access must be managed centrally using IAM groups and policies

---

## Key concepts explored
- IAM users and groups
- Least-privilege access
- AWS managed IAM policies
- Read-only permissions
- IAM security fundamentals
- MFA and access credentials

---

## Observations
- IAM permissions are best managed through groups rather than individuals users
- AWS managed policies such as AmazonEC2readOnlyAccess simplify permission management
- Users without delete permissions are prevented from terminating EC2 instances
- Separate read-only access can be granted to different services, such as Amazon RDS
- IAM introduces multiple security mechanisms, including MFA and access Keys, to protect accounts

---

## Tool used
- AWS Management Console (GUI)
- AWS Identity and Access Management (IAM)
- Amazon EC2
- Amazon RDS
