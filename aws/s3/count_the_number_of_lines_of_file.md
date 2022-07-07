# Count the number of lines of a file on S3.

Using below command, you can count the number of lines of a file on S3 without downloading that file.

```bash
aws s3 cp s3://bucket-name/file-name.csv - | wc -l
```

When you want to count the number of line of gzipped file, you need to add `gunzip` option.

```bash
aws s3 cp s3://bucket-name/file-name.csv.gz - | wc -l
```
