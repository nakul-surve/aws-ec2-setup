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

## Connect to EC2 using SSH

After launching the EC2 instance, SSH is used to securely connect to the server.

### Prerequisites
- EC2 instance is running
- Key pair (.pem file) downloaded
- Security group allows SSH (port 22)

### Step 1: Set key permissions
chmod 400 my-key.pem
#This ensures the private key is not publicly accessible.


# Step 2: Connect to EC2

ssh -i my-key.pem ubuntu@<EC2_PUBLIC_IP>

Replace:
- my-key.pem → your key pair name
- <EC2_PUBLIC_IP> → EC2 public IPv4 address

 Successful connection
 Once connected, you will be logged into the EC2 Linux server and can start managing the system.

 ##Why SSH is Important

SSH provides a secure way to manage cloud servers remotely and is a core skill for DevOps engineers.
