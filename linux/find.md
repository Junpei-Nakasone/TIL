# find
The `find` command can be used to find files and directories and perform subsequent operations on them.

### Options
- -name: specify the name.
- -type: specify the object type. `f` is file and `d` is directory.
- -maxdepth: specify the depth of the directory search to the current directory.

### example
- Find the directory which has `example` in the directory name. It also specified current directory only.
```bash
find . -maxdepth 1 -name "*example*" -type d
```

- Search a file with specific name.
```bash
find ./ -name
```
