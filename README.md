# cloud-aws
## Cloud Foundation
- AWS Well Architected Framework (What tools are we going to use to achieve it)
  - Security
  - Reliability
  - Operational Excellence
  - Performance Efficiency
  - Cost Optimization
  - Sustainability
- Landing Zone
  - AWS Organizations
      - Design
      - Master billing Account
      - Greenfield Accounts
      - Brownfield Accounts
      - Account Naming Convention
  - AWS Control Tower Factory for Terraform
    - Security Account
    - Log archive Account
    - AWS regions supported
    - Enabling Cloud Trail audit
    - Control Tower Customizations
      - Networking
        - Delete default VPC
        - Creating VPCs and Subnets
      - Service Control Policies
        - Deny access to AWS based on the requested AWS Region
        - Prevent IAM users and roles from making certain changes
        - Prevent IAM users and roles from making specified changes, with an exception for a specified admin role
        - Require MFA to perform an API action
        - Block service access for the root user
        - Prevent member accounts from leaving the organization
        - Prevent users from disabling CloudWatch or altering its configuration
        - Prevent users from disabling AWS Config or changing its rules
        - Prevent users from disabling GuardDuty or modifying its configuration
        - Require a tag on specified created resources
        - Prevent users from deleting Amazon VPC flow logs
        - Prevent any VPC that doesn't already have internet access from getting it
        - Restrict Public S3 buckets creation
      - Cross Account IAM Roles
      - IAM Federated Roles
      - SSO Integration
## Networking
- VPC
  - Number of VPC per account
  - VPC Peering
  - Routing
  - Transit Gateway
  - Direct connect
  - NACL
  - VPC Flowlogs
- Subnets
  - Design
    - Red subnets
    - Yellow subnets
    - Container subnets
    - Green subnets
## Security
- Cloud Custodian
- AWS GuardDuty
- SCP Policies
- IAM Roles
  - Creating Service Link Roles
  - Creating IAM Users
    - When should we create IAM Users
    - IAM Users naming convention
    - Safeguard Access and Secret Key
## Infrastructure As Code
- Terraform
  - Why terragrunt?
  - Provisioning
    - Git branching
    - Infrastructure Governance
    - State file management
    - User data management
  - LCM management using terraform
  - Avoid Drift
## Services
- EC2
  - Spot instances
  - Reserved Instances
  - On-Demand Instances
- S3
  - Bucket Encryption
- RDS
## AMI Engineering
- AMI Build Process
  - Implementing Packer
  - Integrating Ansible with Packer
  - Updating Parameter store with AMI ID
  - Sharing AMI ID's to Multiple Accounts
- Server Hardening - CIS Commandments
  - ARM Platform
    - RedHat
    - Amzn Linux 2
    - Ubuntu
    - Windows 2016
    - Windows 2019
    - EKS Optimized
    - ECS Optimized
  - x86 Platform
    - RedHat
    - Amzn Linux 2
    - Ubuntu
    - Windows 2016
    - Windows 2019
    - EKS Optimized
    - ECS Optimized
  - Supported Marketplace AMI's
- AMI Rollout
  - Current AMI Info
  - Previous AMI Info
  - Updating ASG with latest AMI Info
## Kubernetes
## Cloud Governance
## FinOps
- AWS Cost Management
- CUR Reports
- Tagging
## Cloud Operations
### Backup
- EC2 Snapshots
- RDS Backups
### Monitoring
### Automations
## Cloud Migration

