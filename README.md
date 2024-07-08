# aws-policy-samples
Samples of AWS Policy documents.

There needs to be a license option: **Use at your own risk!**

# IAM Policy Samples

`basic-iam-policy.json`

This policy let people get and manage their own account information.  Without an IAM policy like this, people can't change their passwords, add MFA defices, or similar housekeeping on their own.

The resource line prevents people from modifying or seeing other accounts. 

```json
"Resource": "arn:aws:iam::###-AWS-ACCOUNT-NUMBER-###:user/${aws:username}"
```
