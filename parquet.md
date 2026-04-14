# parquet

Apache Parquet columnar file format — the standard interchange format across this corpus for bulk data movement and analytics.

## Members

- [[Anthea]] — reads pricing parquet files via DuckDB
- [[CGI-Sharp]] — queries parquet files through DuckDB ODBC
- [[Declotter]] — stores training data as parquet
- [[DrPQ]] — CLI search tool for parquet files
- [[ElastiCompare]] — stores downloaded ES indexes as parquet for comparison
- [[ESIndexDownloader]] — converts downloaded JSON to parquet via DuckDB
- [[JordanPrice]] — writes parquet as intermediate format in the pricing pipeline
- [[Mallard]] — reads schema metadata from parquet files
- [[Pallets]] — pallet order analysis from parquet data
- [[ParquetToPostgres]] — migrates parquet data into PostgreSQL
- [[PBI-Liveboards]] — DuckDB WASM queries parquet files in-browser
- [[PriceExtractor]] — loads pricing parquet into PostgreSQL
- [[RocsMiddleware]] — several services read/write parquet
- [[BPQuery]] — reads Keycloak event history from parquet

## Related themes

- [[DuckDB]] — the engine most often used to query parquet files
- [[ODBC]] — DuckDB accessed via ODBC in many of these projects
- [[csharp]] — most parquet producers/consumers are .NET
