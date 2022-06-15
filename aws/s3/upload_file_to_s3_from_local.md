# Upload a file to S3 from local computer

You can upload a file to S3 with AWS CLI command. You need provide to arguments which specifies source and destination.

For example, to upload the file on ./local/log.csv to the root of the example bucket, you can use the command below.

```bash
aws s3 cp ./local/log.csv s3://example/
```
First argument is path of local file and second argument is path of S3 destination.
