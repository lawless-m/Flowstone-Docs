# ElastiCompare

A [[csharp]] tool for comparing [[elasticsearch]] indexes between production and staging to validate new indexing programs.

**Repo:** `~/Git/ElastiCompare`

ElastiCompare downloads indexes from two [[elasticsearch]] 5.2 clusters in parallel using the slice/scroll API, stores them as [[parquet]] files, then compares documents field-by-field via [[DuckDB]]. Uses xxHash64 for efficient document hashing and reports exactly which fields differ between source and destination. Strict comparison — no type coercion, case-sensitive, null primary keys are critical failures.
