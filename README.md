# AWS 3-Tier High Availability Architecture

## Overview

This project demonstrates the design and implementation of a
3-tier highly available AWS architecture.

## Region

AWS Region:

eu-west-2 (London)

## Network

VPC:

10.0.0.0/16

### Public Subnets

- 10.0.1.0/24
- 10.0.2.0/24

### Application Subnets

- 10.0.10.0/24
- 10.0.11.0/24

### Database Subnets

- 10.0.20.0/24
- 10.0.21.0/24

## Architecture Components

- Amazon VPC
- Internet Gateway
- NAT Gateway
- Application Load Balancer
- Amazon EC2
- Amazon RDS MySQL
- Amazon S3
- IAM
- Systems Manager


## Security

The application follows a layered security model:

Internet
→ ALB
→ EC2
→ RDS

Security Groups restrict communication between each layer.

## High Availability

The application is distributed across two Availability Zones.

Each AZ contains:

- Public subnet
- Application subnet


The application layer contains EC2 instances in both AZs.


## Documentation

See the documentation directory for detailed network
and security configuration.

## Status

Completed