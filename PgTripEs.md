# PgTripEs

A [[CSharp]] synchronisation service that pushes price_discount changes from PostgreSQL into [[ElasticSearch]].

**Repo:** `~/Git/PgTripEs`

PgTripEs monitors the `price_discount` table in PostgreSQL for action flags (UPD/DEL) and bulk-syncs changes into an [[ElasticSearch]] index. Uses xxHash64 for deterministic document IDs and batch processing (default 1000). Part of the pricing data pipeline alongside [[JordanPrice]] and [[ParquetToPostgres]].
