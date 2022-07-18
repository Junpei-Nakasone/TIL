# lsof command

lsof(list open files) shows all open files and processes that opened them.

### List all open files
```bash
$ lsof
```

### Find who is using a file
```bash
$ lsof /path/to/file
```

### Find who is using a port(for example 8080)
```bash
$ lsof -i:8080
```
