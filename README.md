# Highly Available Web Application on AWS

## Overview
Built a highly available architecture on AWS to handle instance failure without downtime.

## Architecture
- Application Load Balancer (ALB)
- EC2 instances across multiple Availability Zones
- Auto Scaling Group

## Flow
User → ALB → EC2

## What I Did
- Configured ALB to distribute traffic across instances
- Deployed EC2 instances in multiple AZs
- Set up Auto Scaling for fault tolerance

## Testing
- Manually terminated one EC2 instance
- Observed traffic still served via Load Balancer
- Auto Scaling launched a new instance automatically

## Screenshots
- Before Failover → screenshots/failover-before.png
- After Failover → screenshots/failover-after.png
- EC2 Instances → screenshots/ec2-instances.png
- Target Group → screenshots/target-group.png
- Application Output → screenshots/app-output.png

## Key Learning
- Real understanding of high availability
- Importance of Auto Scaling in failure handling
- Load balancing behavior during instance failure
