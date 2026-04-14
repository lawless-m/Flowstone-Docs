# PgTripEs

A [[csharp]] synchronisation service that pushes price_discount changes from PostgreSQL into [[elasticsearch]].

**Repo:** `~/Git/PgTripEs`
**Themes:** [[csharp]], [[dotnet]], [[elasticsearch]]

PgTripEs monitors the `price_discount` table in PostgreSQL for action flags (UPD/DEL) and bulk-syncs changes into an [[elasticsearch]] index. Uses xxHash64 for deterministic document IDs and batch processing (default 1000). Part of the pricing data pipeline alongside [[JordanPrice]] and [[ParquetToPostgres]].
