# Ansible AWS EC2 Provisioning

This repository contains a minimal Ansible playbook that provisions an EC2 instance in AWS using the AWS API.

The playbook runs locally and does **not** require SSH access to AWS.

---

## Requirements

- Ansible 2.13+
- Python 3.9+
- AWS credentials configured via environment variables:
  - `AWS_ACCESS_KEY_ID`
  - `AWS_SECRET_ACCESS_KEY`
  - `AWS_DEFAULT_REGION`
- Python dependencies:
  - boto3
  - botocore

---

## Install Dependencies

```bash
pip install boto3 botocore
ansible-galaxy collection install amazon.aws
