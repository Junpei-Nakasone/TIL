# Renew certification

#### Private
If the domain which used certification issued by AWS ACM can't be accessed from public, ACM won't renew certification automatically.
In that case, the network administrator will receive email from AWS which contains "I approve" button.

You can renew ACM certificate to push that button.

#### Public
ACM will renew your certificate automatically.

#### Certificate's ARN
When ACM renews a certificate, the certificate's ARN(Amazon Resource Name) remains the same.
