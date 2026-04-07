# 3-Tier Web Application on AWS (EC2)

## Overview

This project demonstrates deployment of a 3-tier web application using AWS infrastructure with secure networking and domain mapping.

## Architecture

* **Frontend Layer**: HTML (served via Apache)
* **Application Layer**: PHP-based backend
* **Database Layer**: MySQL (connected to application)

## AWS Infrastructure

* **EC2 (Private Instance)**: Hosts application (no public IP)
* **Bastion Host**: Secure SSH access to private EC2
* **Security Groups**: Controlled access between layers
* **Route 53**: Domain routing and DNS management

## Key Features

* Secure architecture using private EC2
* Bastion-based SSH access (no direct public exposure)
* Domain configured via Route 53
* Real-world production-like setup

## Deployment Steps

1. Created VPC with public & private subnets
2. Launched bastion host in public subnet
3. Launched private EC2 instance for application
4. Configured security groups (SSH via bastion only)
5. Installed Apache & deployed PHP application
6. Connected application to database
7. Configured domain using Route 53

## Learnings

* Secure AWS architecture design
* SSH tunneling via bastion host
* Real-world deployment challenges
* Git + EC2 integration workflow

## Future Improvements

* Containerization using Docker
* CI/CD pipeline using GitHub Actions
* Monitoring using CloudWatch

