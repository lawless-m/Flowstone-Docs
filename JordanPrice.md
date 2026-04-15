# JordanPrice

A [[csharp]] price discount indexer that pipelines data from [[ExportMaster]] through [[Parquet]] and PostgreSQL into [[ElasticSearch]].

**Repo:** `~/Git/JordanPrice`

JordanPrice is a C# port of an original Java implementation. It exports pricing data from [[ExportMaster]] via [[ODBC]], processes it through [[DuckDB]] for a 13x speedup on date calculations, stores it in PostgreSQL, and bulk-indexes to [[ElasticSearch]] with zero-downtime alias swaps. Parallel indexing across CPU cores gives a 4x throughput improvement. Writes [[Parquet]] files as an intermediate format.
