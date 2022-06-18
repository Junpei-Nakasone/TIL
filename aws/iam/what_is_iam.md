# IAM

IAM stands for Identity and Access Management.
It helps you securely control access to AWS resources.

## Features

### Shared access to your AWS account
With IAM permissions, you can grand other people to use AWS resources in your AWS account without using password or access key.

## Difference of root account and IAM user

#### Root account
- There's only one root account for each AWS account number.
- Root account can access every AWS resources on that account.
- You should avoid to use root account for your daily tasks.

#### IAM user
- You can create multiple IAM user for your AWS account.
- IAM user can execute the process which permitted in IAM policies that
linked with it.
- You highly recommended to use IAM user for your daily tasks.
- Usually IAM user is created for each actual user.

