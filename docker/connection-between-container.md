You need to specify container name when you want to make connection between multiple containers.

For instance, if golang application container try to connect MySQL DB container, `localhost` doesn't work and need to specify container name.
```go
// error
db, err := sql.Open("mysql", "root:root@tcp(localhost:3306)/test_database?parseTime=true")

// OK
db, err := sql.Open("mysql", "root:root@tcp(mysql_container:3306)/test_database?parseTime=true")
```
