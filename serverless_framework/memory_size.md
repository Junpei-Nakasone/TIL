You can define memory size of your lambda function like below `memorySize` parameter.

```yaml
service: service-name
provider:
    name: aws
    runtime: python3.9
    memorySize: 512
```

`memorySize` parameter is optional. That is defined in MB, and default is 1024.
