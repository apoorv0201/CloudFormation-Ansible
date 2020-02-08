# CloudFormation-Ansible
Cloud formation template used to provision resources and install JIRA using Asible playbooks
# Ansible

## Installation

sudo yum install python

sudo yum install ansible

sudo yum install java-1.8.0

## Usage

We have install Ansible to run ansible playbook. Using ansible we are installing JIRA software on EC2 instance. 

# Cloudformation

## Template

We have yaml template through which we are provisioning below resources

1. EC2 Instance (t3.large)
2. Security Group to host JIRA
3. RDS instance (db.t2.medium)
4. Ansible playbook inside template will install the JIRA

## How to use template

1. Open Cloudformation Service in AWS console.
2. Click on Create Stack.
3. Now, upload the yaml template
4. Fill the inputs as required ( Enter the Stack Name, DBUserName , DBPassword)
5. Create

## Usage
1. We have used Amazon Linux image to setup the infrastructure.
2. We have provisioned our resources in US East (N. Virginia) us-east-1.
3. A user needs to use the existing Key Pair Name or can generate new key pair
4. Our cloudformation template automatically list down the VPC's which are present in the AWS account.
5. We are running a script which updates the DNS name for the IP. We have to add the IP address in the script.

## How to Generate a Key Pair
1. Go to EC2 instance.
2. Select Key Pair from left side pane.
3. Click on Create Key Pair.
4. Give your key a name and download it in PPK (windows) or PEM (other than windows)
