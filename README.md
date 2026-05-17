# Infrastructure Requests

App teams raise GitHub Issues here to request new AWS infrastructure.

## How to raise a request
1. Click **New Issue** and select the **Infrastructure Request** template
2. Fill in all fields in the table
3. Submit the issue — your manager will review and add the `approved` label
4. Once approved, the MCP server automates the rest

## What happens after approval
1. AWS account created in the correct OU
2. Account registered in Netbox
3. Log account pipeline runs
4. TGW pipeline runs
5. Network infra pipeline runs (VPC, subnets, NAT, KMS, SGs)
6. App infra pipeline runs
7. Issue closed with full resource summary

## Labels
| Label | Meaning |
|---|---|
| `infra-request` | New request raised by app team |
| `approved` | Manager approved — triggers automation |
| `in-progress` | MCP is actively building the infra |
| `module-update` | New Terraform module version available |
