# Three-Tier Web Application Architecture using AWS

## Project Overview

This project demonstrates the design and deployment of a secure and scalable three-tier web application architecture using Amazon Web Services (AWS).

The application is divided into three layers:

1. Web Tier
2. Application Tier
3. Database Tier

## Architecture

User
   |
   v
Application Load Balancer
   |
   v
Web Tier - EC2 (Public Subnet)
   |
   v
Application Tier - EC2 (Private Subnet)
   |
   v
Database Tier - Amazon RDS (Private Subnet)

## AWS Services Used

- Amazon VPC
- Amazon EC2
- Amazon RDS (MySQL)
- Application Load Balancer
- Internet Gateway
- NAT Gateway
- Route Tables
- Security Groups
- Auto Scaling
- Public and Private Subnets

## Implementation

### 1. VPC Configuration
Created a VPC with public and private subnets to isolate different application components.
Deployed EC2 instances in public subnets to handle incoming web requests through the Application Load Balancer.
Deployed application servers in private subnets to process application logic without direct Internet access.
Configured Amazon RDS in a private subnet to securely store application data.
Configured Security Groups to control communication between the three tiers.
Used Application Load Balancer to distribute incoming traffic and Auto Scaling to support application scalability.

- Secure network architecture
- Public and private subnet isolation
- Load balancing
- Scalable infrastructure
- Database security
- Controlled communication between tiers
- High availability

Successfully designed a three-tier cloud architecture that separates web, application, and database resources while providing improved security, scalability, and maintainability.

## Author

Your Name
