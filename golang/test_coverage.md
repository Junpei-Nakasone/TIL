Calculate test coverage with `-cover` option.

```bash
go test -cover ./...
```

Specify which code / conditions is not covered.
Output coverage detail to file named cover.out.
```bash
go test -cover ./... -coverprofile=cover.out
```

With go tool, generate cover.html
```bash
go tool cover -html=cover.out -o cover.html
```
