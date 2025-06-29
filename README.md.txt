Project 2: AWS GuardDuty Threat Detection
This project shows a hands-on use of Amazon GuardDuty to detect a simulated crypto-mining threat in an AWS environment. It was done using AWS Free Tier resources and focused on understanding how GuardDuty identifies suspicious activity.

🔍 Simulated Threat Finding
Finding: CryptoCurrency:EC2/BitcoinTool.B

"The EC2 instance i-99999999 is communicating with a known Bitcoin-related IP address."

This is a high-severity simulated finding. It suggests the EC2 instance might be compromised and used for cryptocurrency mining, which is a common cloud security issue.

📂 Artifact Included
guardduty-finding-bitcoin.json: Raw JSON output showing the threat data captured by GuardDuty.

🧰 Tools Used
Amazon GuardDuty

AWS CLI (via CloudShell)

AWS Identity and Access Management (IAM)

AWS CloudTrail

🎯 Skills Demonstrated
Threat detection with GuardDuty

Investigated simulated threat findings in JSON format

Used AWS CLI to manage services in a secure environment

Configured IAM roles and understood permissions

Tracked and reviewed events using CloudTrail
