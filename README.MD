This project is for Deploying Multi-Node Kubernetes cluster on AWS using Ansible Automation
Requirements:
1. Generate and save an AWS access key and secret
2. Install following packages on your local machine
```
apt-get update
apt-get install python3 pyhton3-pip ansible awscli
pip3 install boto boto3
```
3. Replace access key and secret on file `./inventory/aws_ec2.yaml`
