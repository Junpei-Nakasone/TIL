# Redirect

You can output the result of your standard input (stdin) to file by using `>`. That is called redirect.

example:
```
ls > output_of_ls
```

After execute the command, output_of_ls will be created on your current directory and contains result of `ls` command.

If a file which has same name already exists, content of the file will be overwrite.
To avoid overwrite and want to add new line, you can use `>>`(append) for the command.
