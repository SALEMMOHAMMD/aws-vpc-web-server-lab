# AWS VPC and EC2 Web Server Deployment

## Project Overview
This project demonstrates how to build a custom network infrastructure using Amazon Virtual Private Cloud (VPC) and deploy a web server using Amazon EC2.

## Architecture Components
- **Amazon VPC:** Custom virtual network (10.0.0.0/16).
- **Public Subnets:** Host resources that require internet access.
- **Private Subnets:** Isolate internal resources.
- **Internet Gateway (IGW):** Enables internet connectivity for public subnets.
- **NAT Gateway:** Allows private subnet resources to access the internet.
- **Route Tables:** Control network traffic routing.
- **Security Group:** Allows inbound HTTP traffic.
- **Amazon EC2:** Hosts the web server using Amazon Linux 2023.

## Network Configuration

| Resource | Configuration |
|---|---|
| VPC | lab-vpc |
| VPC CIDR | 10.0.0.0/16 |
| Public Subnet 1 | 10.0.0.0/24 |
| Private Subnet 1 | 10.0.1.0/24 |
| Public Subnet 2 | 10.0.2.0/24 |
| Private Subnet 2 | 10.0.3.0/24 |
| Region | us-east-1 | 

## Security Configuration
- Created a Security Group named `Web Security Group`.
- Configured inbound HTTP access on port 80.
- Allowed HTTP traffic from Anywhere-IPv4.

## EC2 Configuration
- Instance Name: Web Server 1
- AMI: Amazon Linux 2023
- Instance Type: t2.micro
- Web Server: Apache HTTP Server
- Application: PHP Web Application

## Learning Outcomes
- Creating and configuring a custom VPC.
- Understanding public and private subnets.
- Configuring route tables and subnet associations.
- Understanding Internet Gateway and NAT Gateway.
- Managing inbound traffic using Security Groups.
- Deploying a web server on Amazon EC2.

## Project Status
Completed successfully.
 
