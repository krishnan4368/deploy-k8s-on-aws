This project is for Deploying Multi-Node Kubernetes cluster on AWS using Ansible Automation
Kluster will be deployed in ec2 instances with ubuntu OS
Requirements:
1. Generate and save an AWS access key and secret
2. Install following packages on your local machine
```
apt-get update
apt-get install python3 python3-pip ansible awscli
pip3 install boto boto3
ansible-galaxy collection install amazon.aws
```
3. Copy following content and Replace access key and secret with yours into file `./inventory/aws_ec2.yaml`
```
---
  plugin: amazon.aws.aws_ec2
  aws_access_key: <replace wiht your aws key>
  aws_secret_key: <replace with your aws secret>
  region: 
  - ap-south-1 
  keyed_groups:
    - key: tags.Env
      prefix: tag_Env
    - key: tags.Role
      prefix: tag_Role
```      
