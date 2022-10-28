# How to check the charset

You can check the charset by executing below command.

```bash
nkf -g test.txt
Shift_JIS
```

You can also check newline by adding `--guess` option.

```bash
nkf --guess test.txt
Shift_JIS(CRLF)
```
