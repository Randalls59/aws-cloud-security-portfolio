# Secure AWS Foundations Lab

The first project. I built a small AWS security lab from scratch — IAM, S3, VPC, EC2, CloudTrail, and CloudWatch. Each service is configured with a specific security reason behind it, documented here.

## What I built

- IAM users, a group, and a least-privilege policy
- S3 bucket with versioning, encryption, and public access blocked
- Custom VPC with public and private subnets
- EC2 instance — SSH locked to my IP only
- CloudTrail logging all API calls to S3
- CloudWatch alarm on EC2 CPU with email alert

## Docs

- [Architecture](./architecture-diagram.md)
- [Setup](./setup.md)
- [Teardown](./teardown.md)
- [Security Decisions](./security-decisions.md)
- [Interview Q&A](./interview-questions.md)
- [Lessons Learned](./lessons-learned.md)
- [Screenshots](./screenshots/checklist.md)
