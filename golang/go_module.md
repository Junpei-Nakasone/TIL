# Go Modules

A module is a collection of Go packages stored in a file tree with a `go.mod` file at its root.
The `go.mod` file defines the module's path which is also the import path used for the root directory, and its dependency requirements, which are the other modules needed for a successful build.

You can start your module using below `go mod init` command.

```bash
go mod init
```


### go mod tidy
`go mod tidy` command deletes unused modules.
```bash
go mod tidy
```

