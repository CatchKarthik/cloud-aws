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
      - Accounts Design and Structure
        - Account Naming Convention
        - Master billing Account
        - Greenfield Accounts
          - Shared Services
          - Security Account
          - Log archive Account
        - Brownfield Accounts
  - AWS Control Tower Factory for Terraform
    - Vending Multi-AWS Accounts
    - AWS regions supported
    - Enabling Cloud Trail audit
    - Control Tower Customizations
      - Networking
        - Delete default VPC
        - Creating VPCs and Subnets
      - Service Control Policies (Examples below)
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
      - Onboarding applications and requesting access to accounts
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
## DNS
- Route53
  - Hosted Zones
  - Centralized Route53 Management
  - Updating and managing Route53 records
## Security
- AWS GuardDuty
- SCP Policies
- IAM Roles and policies 
  - Creating Service Link Roles
  - Creating IAM Users
    - When should we create IAM Users
    - IAM Users naming convention
    - Safeguard Access and Secret Key
  - IAM Roles - Quarterly Cleanup
- KMS Keys
- Certificate Management
- Secrets Management
## Infrastructure As Code
- Design
  - Tools used for provisioning
  - Self Serve Provisioning
  - Infrastructure Governance
    - Open Policy Agent
    - SNOW Tickets
    - Approvals and RBAC
    - Integrations with other team (Infosec)
  - Drift Detection and avoidance
- Terraform
  - Why terragrunt?
  - Terraform Modules
    - Productizing Modules
    - User data Management using Ansible
    - Versioning Modules 
    - Modules Collections
  - IaC Provisioning
    - Git branching
    - Terraform Stages
    - State file management
    - Lock Management
    - IAM Roles
  - Life Cycle Management
- AWS CloudFormation
  - Productizing CFT's
    - Service Catalog Framework
      - Portfolio
      - Products
      - Drift Detection
      - Updating Products 
    - IAM roles for Provisioning 
    - CFN_NAG 
## AMI Engineering
- AMI Build Process 
  - Tools used to build AMI
  - EC2 Image Builder
  - Packer
    - Implementing Packer
    - Integrating Ansible with Packer
    - Updating Parameter store with AMI ID
    - Sharing AMI ID's to Multiple Accounts
  - AMI Rollout
    - Current AMI Info
    - Previous AMI Info
    - Updating ASG with latest AMI Info
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
## Kubernetes
## Cloud Governance
- Cloud Custodian
- Encryption
  - Data at rest
  - In flight 
- Disaster Recovery
- Data Replication
- Backup
  - Backups Retention
  - Tag Based backup
  - EC2 Snapshots
  - RDS Backups
## FinOps
- Finops Dashboard
- AWS Cost Management
  - Cost and Budget reporting
  - CUR Reports
- Tag Compliance Policies
- Cost Optimization
  - Shutdown and startup of Ec2 based on tags
  - Monitor under-utilized servers
  - Reserved Instances
  - RightSizing Recommendations
## Monitoring
- Tools used for Monitoring
  - AWS Cloudwatch
  - Dynatrace
  - Splunk
  - ELK
- Alert Management
## Automations
- Tools used for Automations
- Lambda
- Configuration Management
  - Why Ansible?
  - Getting access to Ansible AWX
  - Ansible AWX Administration
    - Organizing Projects and templates
    - RBAC Controls in AWX
    - Inventory Management
      - Tag based inventory management
    - Configuration as Code for AWX
    - SSO Integration
    - SNOW Integration
    - Creating Workflow Jobs
  - Playbooks in version control
  - Role Based structure


