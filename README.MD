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
To deploy cluster on aws run command
```
ansible-playbook deploy-k8s.yaml
```
