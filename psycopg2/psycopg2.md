
#### Connect to Redshift
```python
conn = psycopg2.connect(
  host = redshift.host,
  database = database_name,
  port = port,
  user = user_name,
  password = password
)
```

#### execute query

```python
cur = conn.cursor()

query = "select * from example_table"

cur.execute(query)
```

#### Fetch data

```python
data = cur.fechall()
```

