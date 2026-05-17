---
name: 'aws-cost-cleanup'
description: 'Automated cleanup of unused AWS resources to reduce costs'
adopted: 2026-05-16
batch: bulk-adoption
source: antigravity-awesome-skills
tier: 4
version: 1.0.0
---

# aws-cost-cleanup

"Automated cleanup of unused AWS resources to reduce costs"

## When to Use

- Use this skill when working on tasks related to aws cost cleanup
- Apply best practices from antigravity-awesome-skills

## Workflow

name: aws-cost-cleanup
description: "Automated cleanup of unused AWS resources to reduce costs"
risk: safe
source: community
date_added: "2026-02-27"
# AWS Cost Cleanup
Automate the identification and removal of unused AWS resources to eliminate waste.
## When to Use This Skill
Use this skill when you need to automatically clean up unused AWS resources to reduce costs and eliminate waste.
## Automated Cleanup Targets
**Storage**
- Unattached EBS volumes
- Old EBS snapshots (>90 days)
- Incomplete multipart S3 uploads
- Old S3 versions in versioned buckets

## Source

Adopted from: antigravity-awesome-skills
