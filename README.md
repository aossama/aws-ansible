A small framework for automating Ansible with AWS CloudFormation.

## Overview
The purpose of this repo is to have a small framework of ansible playbooks work in conjuction with AWS CloudFormation to facilitate the provisioning and automating infrastructures.

### Region
The default region is us-east-1 but can be changed when running the aws.py script by specifying --region=us-west-2 for example. The region must contain at least 3 Availability Zones.

Before running aws.py
 
```bash
$ virtualenv -p python3 venv
$ source venv/bin/activate
$ pip install --upgrade pip setuptools
$ pip install -r requirements.txt
```

## Usage
```bash
./aws.py --keypair=my-aws-kp --public-hosted-zone=my-aws.local
```