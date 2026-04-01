# AWS Cheat Sheet

## ⚙️ Setup
- `aws configure` → Configure credentials

## 📦 S3
- `aws s3 ls` → List buckets
- `aws s3 cp file s3://bucket/` → Upload file
- `aws s3 sync . s3://bucket/` → Sync directory

## 💻 EC2
- `aws ec2 describe-instances` → List instances
- `aws ec2 start-instances --instance-ids id` → Start
- `aws ec2 stop-instances --instance-ids id` → Stop

## 🔐 IAM
- `aws iam list-users` → List users

## 📜 Logs
- `aws logs describe-log-groups` → List logs