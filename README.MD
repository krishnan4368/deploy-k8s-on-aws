This project is for Deploying Multi-Node Kubernetes cluster on AWS using Ansible Automation
Cluster will run on Ubuntu 22.04 OS, uses CRI-O as container runtime and uses kubeadm.
Requirements:
1. Generate and save an AWS access key and secret
2. Install following packages on your local machine
```
apt-get update
apt-get install python3 pyhton3-pip ansible awscli
pip3 install boto boto3
```
3. Make sure to update `group_vars/all` file with your preferd values
4. Run following command to initalize cluster `ansible-playbook deploy-k8s.yaml`
