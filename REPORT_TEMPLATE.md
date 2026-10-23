# AWS VPC Peering Project Report

**Student:** [Your name]  
**Date:** [Completion date]  
**AWS Region:** [Region]  
**GitHub URL:** [Repository URL]  
**Implementation status:** [In progress / Completed and verified]

> Fill this report only with observations from your own deployment. Do not mark tests successful unless you ran them.

## 1. Objective
Explain why VPC Peering is used and what you intended to demonstrate.

## 2. Architecture
Insert `docs/images/architecture.png`. Explain VPC A, VPC B, subnets, bastion, private instances, and peering.

## 3. Resource inventory
Record actual resource IDs, CIDRs, private IPs, and states from the AWS Console. Replace planned values where needed.

## 4. Routes and security
Document route tables, subnet associations, security group rules, and why SSH is limited to a trusted source.

## 5. Results

| Test | Expected | Actual result | Screenshot filename |
|---|---|---|---|
| Baseline cross-VPC ping before routes/peering | Usually fails | [Observed] | `01-...` |
| App A → App B after configuration | Success if all rules correct | [Observed] | [Filename] |
| App B → App A after configuration | Success if all rules correct | [Observed] | [Filename] |
| Remove ICMP rule and retry | Failure | [Observed] | [Filename] |
| Restore ICMP rule and retry | Success | [Observed] | [Filename] |

## 6. Troubleshooting
For each issue, record the symptom, checks, root cause, and fix.

## 7. Cost and cleanup
List the resources removed, attach cleanup evidence, and confirm the Billing console has no unexpected lab resources.

## 8. What I learned
Describe CIDR planning, route tables, peering, security groups, bastion access, troubleshooting, and cost controls in your own words.
