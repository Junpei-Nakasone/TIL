# du command

The `du` command is a standard Linux/Unix command that allows a user to gain disk usage information.
`du` command has various options to make it easy to understand for users.

### -h, --human-readable
The `-h` flag prints size outputs,

```bash
du -h example-directory/
 24K	example-directory//.vscode
787M	example-directory/
```

### -s, --summarize
The `-s` flag outputs total disk usage.
Also, `-s` option can be used with `-h` option so that result would be easy to understand.

```bash
du -sh example-directory/
787M	example-directory/
```
