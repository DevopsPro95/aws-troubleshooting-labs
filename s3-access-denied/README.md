# S3 Access Denied Troubleshooting

## Common Causes
- IAM user/role missing s3:GetObject or s3:ListBucket permissions
- Bucket policy explicitly denies access
- S3 Block Public Access enabled
- KMS encryption permissions missing (kms:Decrypt)

## Basic Checks

### 1. Test access using AWS CLI
```bash
aws s3 ls s3://your-bucket-name
