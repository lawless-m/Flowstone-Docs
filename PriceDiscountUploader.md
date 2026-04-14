# PriceDiscountUploader

A [[RocsMiddleware]] service that pushes price discount changes from PostgreSQL into [[elasticsearch]].

**Repo:** `~/Git/RocsMiddleware/PriceDiscountUploader`
**Themes:** [[csharp]], [[dotnet]], [[elasticsearch]]

Reads action flags (DEL/UPD/NEW) from PostgreSQL `rocs.price_discount`, batch-deletes and batch-indexes into the [[elasticsearch]] `price_discount` index, then clears the flags.
