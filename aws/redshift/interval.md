
```sql
SELECT to_date('2022-06-24', 'YYYY-MM-DD') - interval '1 month'

-- 2022-05-24 00:00:00.000

SELECT to_date('2022-06-24', 'YYYY-MM-DD') - interval '1 day'

-- 2022-06-23 00:00:00.000
```
