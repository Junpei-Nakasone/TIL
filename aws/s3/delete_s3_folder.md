# Delete a folder from an S3 bucket

You can delete a folder from S3 bucket by below AWS CLI command.
`--recursive` parameter applies the action to all files under given s3 path.

```bash
aws s3 rm s3://bucket-name/path/to/folder --recursive
```
