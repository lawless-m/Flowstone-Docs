# PriceExtractor

A [[RocsMiddleware]] overnight batch service that loads pricing data from [[Parquet]] files into PostgreSQL via [[DuckDB]].

**Repo:** `~/Git/RocsMiddleware/PriceExtractor`

Reads price discount parquet files through [[DuckDB]], queries [[Elasticsearch]] for the current pricing period, and upserts into PostgreSQL `rocs.price_discount` with hash-based change tracking. Supports full and per-customer incremental modes.
