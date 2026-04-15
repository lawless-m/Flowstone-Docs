# PriceDiscountUploader

A [[RocsMiddleware]] service that pushes price discount changes from PostgreSQL into [[ElasticSearch]].

**Repo:** `~/Git/RocsMiddleware/PriceDiscountUploader`

Reads action flags (DEL/UPD/NEW) from PostgreSQL `rocs.price_discount`, batch-deletes and batch-indexes into the [[ElasticSearch]] `price_discount` index, then clears the flags.
