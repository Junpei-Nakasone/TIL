
Create table with same table structure as existing other table.
By below statement, new_table will be empty.
```sql
CREATE TABLE IF NOT EXISTS new_table (like existing_table);
```

By below, new_table will have same data as existing_table.

```sql
CREATE TABLE new_table AS SELECT * FROM existing_table;
```
