# InvoiceUploader

A [[RocsMiddleware]] service that uploads invoices from PostgreSQL to [[sage-x3]] via its REST API.

**Repo:** `~/Git/RocsMiddleware/InvoiceUploader`
**Themes:** [[csharp]], [[dotnet]], [[sage-x3]]

Reads unprocessed invoices from PostgreSQL, generates JSON payloads via a stored procedure, posts to the X3 Customer BP Invoice endpoint with a 250ms delay between calls, and records X3 document numbers or failures back to the database.

## Related

- [[RocsMiddleware]]
- [[InvoiceExtractor]] — upstream: extracts invoices from ExportMaster into PostgreSQL
- [[sage-x3]]
