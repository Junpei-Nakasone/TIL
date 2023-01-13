Serverless framework allows you to specify different stages to deploy your project to. Changing the stage will change the environment your function is running on, which is helpful when you wish to keep production code partitioned from your development environment.


### Refer the stage from CLI option
If you want to refer the stage from CLI option, you can use `${opt:VAR_NAME}` syntax in serverless.yml file like below.

```yaml
service: example-project
frameworkVersion: '3'

provider:
  name: aws
  runtime: python3.8
  memorySize: 128
  timeout: 60
  stage: ${opt:stage}
```
When you execute `sls deploy --stage dev`, `${opt:stage}` returns `dev`.
Also, when you execute `sls deploy --stage prd`, `${opt:stage}` returns `prd`.
