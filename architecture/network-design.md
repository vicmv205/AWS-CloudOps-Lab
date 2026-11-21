# AWS Network Architecture

## Objective

Design and configure an AWS network environment with public and private EC2 instances, controlled network access, and secure communication between instances.

## Infrastructure Components

- **VPC:** Custom virtual private cloud
- **Public Subnet:** Hosts an EC2 instance with internet connectivity
- **Private Subnet:** Hosts an EC2 instance without direct internet connectivity
- **Internet Gateway:** Provides internet access through the public subnet's route table
- **Route Tables:** Control traffic routing
- **Security Groups:** Restrict inbound and outbound traffic

## Network Configuration

### Public Subnet

- Associated with a route table containing a default route to the Internet Gateway.
- Hosts a public EC2 instance.
- Configured for controlled SSH access.

### Private Subnet

- Associated with a route table containing the VPC local route.
- Hosts a private EC2 instance.
- Does not have a default route to an Internet Gateway or NAT Gateway.
- Permits authorized communication from the public EC2 instance.

## Instance Communication

The public EC2 instance communicates with the private EC2 instance using its private IP address over TCP port 8080.

Communication within the VPC uses the local route, while security group rules control which connections are permitted.

## Verification

- Verified SSH connectivity to the public EC2 instance.
- Verified internal network communication between EC2 instances.
- Confirmed the private subnet has no direct route to the internet.

## Security Design

The private EC2 instance is isolated from direct inbound internet access. Access to the private service is restricted through security group rules.

This architecture demonstrates network segmentation, access control, and foundational AWS networking principles.
