# InvoiceExtractor

A [[RocsMiddleware]] service that extracts invoices from [[ExportMaster]] and stores them in PostgreSQL for X3 upload.

**Repo:** `~/Git/RocsMiddleware/InvoiceExtractor`
**Themes:** [[csharp]], [[dotnet]], [[ExportMaster]], [[ODBC]]

Queries [[ExportMaster]] via [[ODBC]] in batches of 100, enriches with customer dimension data from PostgreSQL, and bulk inserts headers and lines in a single transaction. Smart filtering skips already-extracted invoices.
