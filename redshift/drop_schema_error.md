# drop schema error

If you try to drop schema which has existing table in it, you will be encounter bellow error.

```sql
DROP SCHEMA example_schema
ERROR: cannot drop schema example_schema because other objects depend on it
HINT: Use DROP ... CASCADE to drop the dependent objects too.
```

To avoid above error, you need drop the table before drop schema.

```sql
DROP TABLE example_table
DROP TABLE example_schema
```

Check the dependencies if you still get same error.
