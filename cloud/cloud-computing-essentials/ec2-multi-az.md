# EC2 development Across Multiple Availability Zones

##Description 
This lab involved deployin Amazon EC2 instances using the AWS MAnagement Console and making them publicly accesible via a web browser.

The objective was to understand how EC2 instances are launched, configured and distributed across different Availability Zones within the same AWS Region.

## Steps performed
- Launched an Amazon EC2 instance
- Selected an Amazon Machine Image (AMI)
- Chose an instance type
- Configures a Security Group to allow web access
- Selected a subnet within a specific Availability Zone
- Used a user data scrept to display instance information in a browser
- Accessed the application via the public IP address
- Launched a second EC2 instance in a different Availability Zone of the same region

  ## Key concepts
  - How EC2 instances are deployed and configured
  - How Security Groups control inbound access
  - The relationship between subneets and Availability Zones
  - How deploying instances across multiple AZs improves availability
 
  ## Notes
  - This setup demostrates basic multi-AZ deployment concepts
  - No load balance was used in this lab
  - High availability was achieved conceptually by distributing instances across Azs
 
  ## Additional exploration
  During this lab, I also explored sevreal EC2 operational concepts:

    - Reviewed different instance families, sizes, pricing, and storage characteritics
    - Observed that SSH access was not available due to the absence of a key pair
    - Connected to the instance using EC2 Instance Connect
    - Accessed the instance terminal directly from the AWS Console
    - Navigated the filesystem using basic Linux commands (ls, cd)
    - Inspected system logs using tail
 
  ## User date review
  I reviewed the user data script used during the instance launch, which included:
  
  - A bash shebang (#!/bin/bash)
  - Creation of directories using mkdir
  - copying files from an S3 bucket to the EC2 instance using aws S3 cp
  - Installing PYthon libraries using pip
  - Starting a web service at the end of the script
 
  This demostrated how EC2 instances con be bootstrapped automatically at launch time using user data scripts
  
