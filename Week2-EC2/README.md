AWS Cloud Security Lab - Week 2: EC2 Setup and Security


Overview


In this lab, I worked with an EC2 Linux instance to apply secure best practices. This included patching, hardening SSH, assigning an IAM role, configuring CloudWatch monitoring, and applying tags for easier management.

Steps Completed


✅ 1. Patching & Upgrades
Connected to the EC2 instance via SSH

Updated and upgraded all packages to close vulnerabilities


Ran code: sudo apt update && sudo apt upgrade -y

Why?: Maintain system security by applying the latest updates.

✅ 2. SSH Hardening
Disabled root login by setting PermitRootLogin no

Disabled password authentication with PasswordAuthentication no

Ensured only key-based authentication is allowed

Restarted SSH service to apply changes



Why?: Follows the principle of least privilege and prevents brute-force password attacks.

✅ 3. IAM Role
Created and attached an IAM role with the policy AmazonS3ReadOnlyAccess

Verified the instance could list S3 buckets using the AWS CLI


Ran code: aws s3 ls



Why?: Allows EC2 to securely access S3 using temporary credentials rather than hardcoded keys.

✅ 4. CloudWatch Monitoring
Confirmed default EC2 metrics (CPU, network, disk) were reporting to CloudWatch

Created a CloudWatch alarm for CPU utilization >80%

Practiced alarm creation with no SNS topic



Why?: Enables proactive monitoring and supports operational excellence.

✅ 5. Resource Tagging
Added the following tags to the EC2 instance:

Name: Week2-EC2

Environment: Dev

Owner: YourName



Why?: Helps organize resources, simplify cost tracking, and enable automation.

Lessons Learned


✅ Applying security updates is critical

✅ SSH must be locked down for secure administration

✅ IAM roles remove the need for risky static credentials

✅ CloudWatch is essential for proactive alerting

✅ Tagging supports cost allocation and resource governance

Next Steps (Week 3 Preview)
Deep dive on S3

Bucket policies and encryption

Secure data storage
