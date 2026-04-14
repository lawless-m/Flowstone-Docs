# ParquetToPostgres

A [[csharp]] migration utility that loads price discount data from [[parquet]] files via [[DuckDB]] into PostgreSQL.

**Repo:** `~/Git/ParquetToPostgres`
**Themes:** [[csharp]], [[dotnet]], [[parquet]], [[DuckDB]], [[ODBC]]

ParquetToPostgres reads [[parquet]] files through [[DuckDB]] [[ODBC]], parses embedded JSON documents, validates primary keys, and batch-upserts into the `price_discount` table in PostgreSQL on rivsprod01. 5000 records per batch with transaction rollback on error.
