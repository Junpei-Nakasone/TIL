# Oracle rownum

Oracle Database does not have the LIMIT clause like MySQL or Postgresql.

When you want to limit the rows returned by a query, you can use rownum keyword to specify how many rows you want.

```
select * from example_table
where rownum = 10
```

Please note that rownum is evaluated before order by clause. So if you want to use both rownum and order by, consider using subquery.
