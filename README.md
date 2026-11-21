# AWS CloudOps Lab

## Project Overview

This project documents my hands-on experience building, securing, monitoring, and troubleshooting AWS infrastructure.

The objective is to develop practical Cloud Operations skills through real-world infrastructure configurations, Linux administration, incident response, and troubleshooting.

## AWS Services Used

- Amazon VPC
- Amazon EC2
- Amazon CloudWatch
- Internet Gateway
- Route Tables
- Security Groups

## Phase 1 — AWS Networking (Completed)

- Created a custom VPC with public and private subnets.
- Configured route tables and an Internet Gateway.
- Deployed public and private EC2 instances.
- Configured security groups to control traffic.
- Established SSH access to the public EC2 instance.
- Verified communication between public and private EC2 instances while restricting direct internet access to the private subnet.

## CloudWatch Monitoring and Incident Response (Completed)

- Configured a CloudWatch alarm to monitor public EC2 CPU utilization.
- Simulated a high-CPU incident.
- Investigated the affected instance using Linux process-monitoring tools.
- Terminated the offending processes.
- Verified CPU recovery and alarm recovery.

## Phase 2 — Linux Administration (In Progress)

Practicing Linux system administration, process management, file permissions, systemd service management, and troubleshooting.

## Upcoming Work

- Deploy and operate an Nginx web service.
- Troubleshoot service failures and network connectivity.
- Introduce Bash scripting and AWS CLI automation.
- Reproduce infrastructure using Terraform.
- Explore Docker and basic CI/CD workflows.
