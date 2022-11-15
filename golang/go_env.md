By using `go env` command, you can see all environmental variables that golang uses.
```go
$ go env
```

You can all so print out specific environmental variables by adding variable name.

```bash
$ go env GOOS
darwin

$ go env GOOS GOARCH
darwin
amd64
```

# environmental variables on go env

### GO111MODULE


