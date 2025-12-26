# aws-ec2-setup
Steps to launch and secure an AWS EC2 instance

# AWS EC2 Setup –
This repository documents the steps I learned to launch and configure an AWS EC2 instance as part of my DevOps learning.

## Services Used
- AWS EC2
- AWS IAM
- Security Groups

## Steps Covered
1. Create an AWS account
2. Launch EC2 instance
3. Choose AMI and instance type
4. Configure key pair
5. Configure security group (SSH, HTTP)
6. Connect to EC2 using SSH
7. Basic instance management

## What I Learn
- Understanding virtual servers in AWS
- Basics of cloud security
- Importance of IAM and security groups

## Status
Actively learning AWS and updating this repository.


## After Launch – Basic Setup

### Instance Checks
- Verify instance state is running
- Check public IP and connectivity
- Ensure security group allows SSH (port 22)

### Basic Server Setup
- Update packages
  sudo apt update && sudo apt upgrade -y

- Install basic tools
  sudo apt install nginx -y

### Verification
- Access Nginx using public IP in browser
- Confirm default Nginx page loads
