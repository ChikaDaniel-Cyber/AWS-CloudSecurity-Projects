# Week 2 - EC2 Setup and Security Lab

## Overview
In this lab, I launched an EC2 instance using Ubuntu 22.04 LTS on AWS. I configured a security group with least privilege to only allow SSH traffic from my current IP.

## Security Group
- Port: 22 (SSH)
- Source: my IP only
- Outbound: default allow all

## Steps Taken
1. Launched EC2 t2.micro instance
2. Configured SSH key pair
3. Created security group with inbound rule restricted to my IP
4. Connected via SSH with private key
5. Verified OS with uname -a
6. Tested outbound connectivity with ping google.com

## Screenshots
- week2-aws-ec2 
- week2-aws-ec2-a
- week2-aws-ec2-b

## Notes
- Followed the principle of least privilege
- Documented all credentials securely (key file permissions set with chmod 400)
- Will tear down resources after testing to avoid charges
