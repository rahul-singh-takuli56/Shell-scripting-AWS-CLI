# Shell-scripting-AWS-CLI
Shell scripting with the AWS Command Line Interface (CLI) involves using shell scripting languages, such as Bash, to automate interactions with AWS services through the command-line interface.
The AWS CLI provides a set of commands and options that allow you to manage various AWS resources and services from the command line. By combining these commands with shell scripting, you can create powerful automation scripts to perform tasks such as provisioning resources, configuring services, deploying applications, and more.


## Installation

Use the below command to install aws cli

```bash
sudo snap install aws-cli
aws --version 
```

## Usage

```python
#create a file 
vim aws_resource_tracker.sh
#!/bin/bash
# Author: Rahul
# Date: 7th-July
# Version:v1
# This script will report the AWS resourcse usage
# AWS S3
# AWS Lambda
# AWS IAM Users

# list s3 bucket
echo "print list of s3 buckets"
aws s3 ls

# lsit EC2 Instance
echo "print list of ec2 instances"
aws ec2 describe-instances

# list aws lambda function
echo "print list of aws lambda function"
aws lambda list-functions

#list IAM users
echo "print list of IAM users"
aws iam list-users


## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.
