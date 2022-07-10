# Get parameter from ssm


boto3 doc
https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_parameter

```python
import boto3

ssm = boto3.client('ssm', region_name='ap-northeast-1')

ssm.get_parameter(Name='the-parameter-name',
WIthDecryption=True)
```
