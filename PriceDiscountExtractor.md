# PriceDiscountExtractor

A [[RocsMiddleware]] service that pulls price discounts directly from [[sage-x3]] SQL Server into PostgreSQL.

**Repo:** `~/Git/RocsMiddleware/PriceDiscountExtractor`

Workaround for X3's REST API not marking customers as updated when only discounts change. Queries X3 SQL Server directly via [[ODBC]], upserts into PostgreSQL `rocs.price_discount` with incremental (2-hour buffer) or full sync modes.
