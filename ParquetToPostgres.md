# ParquetToPostgres

A [[CSharp]] migration utility that loads price discount data from [[Parquet]] files via [[DuckDB]] into PostgreSQL.

**Repo:** `~/Git/ParquetToPostgres`

ParquetToPostgres reads [[Parquet]] files through [[DuckDB]] [[ODBC]], parses embedded JSON documents, validates primary keys, and batch-upserts into the `price_discount` table in PostgreSQL on rivsprod01. 5000 records per batch with transaction rollback on error.
