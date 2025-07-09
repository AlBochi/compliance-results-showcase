# Saillent SOC 2 Type 2 Engagement Summary
**Client:** Saillent Inc. (AI SaaS Provider)  
**Engagement Period:** June 1 – June 28, 2025  
**Auditor:** [Redacted] Cloud Compliance Advisory  

## Executive Summary
Saillent Inc. required expedited SOC 2 Type 2 certification to meet a contractual deadline with a $4.9M enterprise deal. Pre-assessment revealed gaps in IAM security and evidence logging.

## Critical Findings (Before Remediation)
- IAM misconfigurations (no MFA, wildcard roles)
- No asset inventory or CMDB
- Missing documented security policies

## Technical Remediation Highlights
1. Terraform-based VPC + IAM hardening
2. AWS Config Rules mapped to SOC 2
3. CIS Benchmark applied to EC2 and RDS
4. Real-time audit dashboards via Streamlit

## Outcomes
- Compliance score: 45% → 98%
- 0 audit exceptions in final review
- Contract closed in 27 days
- Reduced audit prep time from 3 months → 21 days

## Confidentiality Notice
Names, architecture diagrams, and identifiers are redacted to preserve client privacy.

---
*Prepared for portfolio demonstration purposes only*
