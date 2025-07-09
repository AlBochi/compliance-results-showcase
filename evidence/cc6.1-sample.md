# Control CC6.1 - Logical Access Security

**Description:** Restrict logical access to information assets

## Implementation Evidence
1. IAM permission boundaries applied to all roles
2. Session Manager used for all administrative access
3. CloudTrail logs encrypted with KMS CMK

```terraform
resource "aws_iam_policy" "developer_boundary" {
  name        = "DeveloperBoundaryPolicy"
  description = "Permission boundary for developer roles"

  policy = jsonencode({
    "Version": "2012-10-17",
    "Statement": [
      {
        "Effect": "Deny",
        "Action": "rds:*",
        "Resource": "*"
      }
    ]
  })
}

