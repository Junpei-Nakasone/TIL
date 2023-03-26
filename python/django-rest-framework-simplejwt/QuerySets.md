In Django, to retrieve objects from your database, construct a QuerySet via Manager on your model class.
A QuerySet represents a collection of pbjects from your database. It can have zero, one or many filters. Filters narrow down the query results based on the given parameters. In SQL terms, a QuerySer equates to SELECT statements, and a filter is a limiting clause such as WHERE or LIMIT.
