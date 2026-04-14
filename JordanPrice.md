# JordanPrice

A [[csharp]] price discount indexer that pipelines data from [[ExportMaster]] through [[parquet]] and PostgreSQL into [[elasticsearch]].

**Repo:** `~/Git/JordanPrice`
**Themes:** [[csharp]], [[dotnet]], [[ExportMaster]], [[elasticsearch]], [[parquet]], [[DuckDB]], [[ODBC]]

JordanPrice is a C# port of an original Java implementation. It exports pricing data from [[ExportMaster]] via [[ODBC]], processes it through [[DuckDB]] for a 13x speedup on date calculations, stores it in PostgreSQL, and bulk-indexes to [[elasticsearch]] with zero-downtime alias swaps. Parallel indexing across CPU cores gives a 4x throughput improvement. Writes [[parquet]] files as an intermediate format.
