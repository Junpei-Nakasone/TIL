# Add a parameter to ssm

You can use put_parameter function when you want to add new parameter to ssm.

```python
import boto3

ssm = boto3.client('ssm')
ssm.put_parameter(
  Name='parameter_name',
  Value='parameter_value',
  Type='string',
  Overwrite=True,
)
```
