# DATE_TRUNC function

The DATE_TRUNC function truncates(shorten the duration or extent of) a timestamp expression or literal based on the date part that you specify, such as hour, day, or month.

### Example
Truncate the input timestamp to the second.

```sql
SELECT DATE_TRUNC('second', TIMESTAMP '20200430 04:05:06.789');
```

|date_trunc|
|--|
|2020-04-30 04:05:06|

Truncate the input timestamp to the minute.

```sql
SELECT DATE_TRUNC('minute', TIMESTAMP '20200430 04:05:06.789');
```

|date_trunc|
|--|
|2020-04-30 04:05:00|
