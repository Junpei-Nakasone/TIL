If you define `id` column in your model, you will encounter bellow error.

```
StandardError: An error has occurred, this and all later migrations canceled:

you can't redefine the primary key column 'id'. To define a custom primary key, pass { id: false } to create_table.
```

That's because `id` column is automatically created by Active Record model as default primary key.
So by adding id column by yourself makes redefining same column error.

To resolve the error, you need remove `id` column from your migration file.
