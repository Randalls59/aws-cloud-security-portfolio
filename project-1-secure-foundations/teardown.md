# Teardown Guide — Project 1

Run these steps in order to avoid orphaned resources and unexpected charges.

## Order of Deletion

1. **CloudWatch** — delete alarms, log groups, SNS topic and subscription
2. **CloudTrail** — stop logging, delete trail
3. **EC2** — terminate instance, delete security group, delete key pair
4. **VPC** — delete subnets, detach and delete IGW, delete route tables, delete VPC
5. **S3** — empty bucket (all objects + all versions), delete bucket
6. **IAM** — remove user from group, delete user, delete group, delete any custom policies

## Verification Checklist
- [ ] EC2 console: 0 running instances
- [ ] S3 console: bucket deleted
- [ ] CloudTrail console: no active trails
- [ ] CloudWatch console: no active alarms
- [ ] Billing dashboard: no unexpected charges
