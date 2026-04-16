# ESIndexDownloader

A [[CSharp]] tool for downloading [[ElasticSearch]] indexes to JSON and converting them to [[Parquet]] via [[DuckDB]].

**Repo:** `~/Git/ESIndexDownloader`

ESIndexDownloader uses the scroll API to bulk-download entire ElasticSearch 5.2 indexes (production and staging) with retry logic and exponential backoff, then pipes the JSON through [[DuckDB]] to produce Parquet files for the data warehouse. Currently focused on the price_discount index.
