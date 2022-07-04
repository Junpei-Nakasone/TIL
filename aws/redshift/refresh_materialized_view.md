# Refreshing a materialized view

When the data in the underlying table is changed, the data in the materialized view remains unchanged.
You can use `REFRESH MATERIALIZED VIEW` to update the data in the materialized view to refresh materialized view.

Amazon Redshift has two types of refreshing method, an incremental refresh and a full refresh.

To automatically refresh materialized view, you can use `AUTO REFRESH`.
