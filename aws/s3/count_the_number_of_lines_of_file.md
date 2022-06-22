# Count the number of lines of a file on S3.

Using below command, you can count the number of lines of a file on S3 without download that file.

```bash
aws s3 cp s3://bucket-name/file-name.csv - | wc -l
```
