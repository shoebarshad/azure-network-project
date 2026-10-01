# Azure Network Project

## Overview
This project deploys a complete Azure networking environment using Terraform.

## Architecture
- Resource Group
- Virutal Network (10.0.0.0/16)
- Subnet (10.0.1.0/24)
- Network Security Group with SSH rule
- Public IP
- Network Interface
- Linux Virtual Machine (Ubuntu 22.04)

## Prerequisites
- Azure subscription
- Terraform installed
- Azure CLI authenticated (`az login`)
- SSH key pair

## How to Deploy
1. Clone this repository
2. Run `terraform init`
3. Run `terraform plan`
4. Run `terraform apply`

## How to Connect
`ssh -i ~/.ssh/azure_vm_key adminuser@<public_ip>`

## How to Destroy
`terraform destroy`

## Skills Demonstrated
- Terraform resource management
- Azure networking (VNet, Subnet, NSG)
- Variables and outputs
- SSH key authentication
- Git and GitHub workflow